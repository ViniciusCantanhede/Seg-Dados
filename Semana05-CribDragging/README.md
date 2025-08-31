# Semana 5 - Crib Dragging Attack

## Objetivo
Demonstrar ataque contra reutilização de chaves em sistemas OTP.

## Como funciona
- Explora a propriedade: C1 ⊕ C2 = P1 ⊕ P2 quando mesma chave é reutilizada
- Usa "berços" (palavras conhecidas) para revelar texto plaintext
- 15 criptogramas disponíveis para análise

## Como executar
```bash
cd src
javac QuebraOTP.java
java QuebraOTP
```

## Uso
1. Digite índice do primeiro criptograma (0-14)
2. Digite índice do segundo criptograma (0-14) 
3. Digite um berço (palavra que você suspeita estar no texto)
4. O programa revelará o texto correspondente no outro criptograma

## Observações
- **NÃO é quebra de OTP verdadeiro** (impossível matematicamente)
- Ataca **reutilização de chave** (vulnerabilidade de implementação)
- Berço deve estar alinhado na mesma posição nos dois textos
- Fundamental para entender por que chaves nunca devem ser reutilizadas
