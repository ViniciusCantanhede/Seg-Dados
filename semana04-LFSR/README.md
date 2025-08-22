# Semana 4 - Linear Feedback Shift Register (LFSR)

## Objetivo
Implementar gerador de números pseudoaleatórios usando LFSR para cifras de fluxo.

## Como funciona
- 3 registradores de 32 bits (cabeça + 2 geradores)
- Cada registrador inicializado com chave de 4 caracteres
- Torneiras XOR em posições específicas para realimentação
- Gera stream de bits convertidos para caracteres ASCII

## Como executar
```bash
cd src
javac LinearFeedbackShiftRegister.java
java LinearFeedbackShiftRegister
```

## Entrada
- 3 chaves de 4 letras cada (uma para cada registrador)

## Observações
- Algoritmo gera 8M de caracteres (pode demorar)
- Base para cifras de fluxo modernas
- Qualidade criptográfica depende da escolha das torneiras
