# Aula 3: Estruturas de Decisão na Lógica de Programação

## Introdução
Na lógica de programação, um algoritmo muitas vezes precisa tomar decisões. Nem sempre o código deve ser executado de cima a baixo, linha por linha, da mesma forma em todas as vezes. As **estruturas de decisão** (ou estruturas condicionais) permitem que o programa escolha qual bloco de código executar com base em uma condição previamente definida.

Essas condições são formadas por expressões lógicas que resultam sempre em valores booleanos: **Verdadeiro** (True) ou **Falso** (False).

## Tipos de Estruturas de Decisão

### 1. Estrutura de Decisão Simples (SE / IF)
É a forma mais básica. O bloco de código interno só será executado se a condição testada for verdadeira. Se for falsa, o programa simplesmente pula esse bloco e continua a execução normalmente na linha seguinte.

**Sintaxe em Pseudocódigo:**
```
SE (condição) ENTAO
    // Executa este bloco de código se a condição for verdadeira
FIM SE
```

**Exemplo:**
```
nota <- 8
SE (nota >= 7) ENTAO
    escreva("Aluno Aprovado")
FIM SE
```

### 2. Estrutura de Decisão Composta (SE... SENAO / IF... ELSE)
Neste caso, estipulamos um caminho alternativo caso a condição principal não seja atendida. Se a condição for verdadeira, o primeiro bloco de código é executado. Se for falsa, o bloco de código atrelado ao "Senão" será executado.

**Sintaxe em Pseudocódigo:**
```
SE (condição) ENTAO
    // Executa este bloco se for verdadeiro
SENAO
    // Executa este bloco se for falso
FIM SE
```

**Exemplo:**
```
nota <- 5
SE (nota >= 7) ENTAO
    escreva("Aluno Aprovado")
SENAO
    escreva("Aluno Reprovado")
FIM SE
```

### 3. Estrutura de Decisão Encadeada (SE... SENAO SE / IF... ELSE IF)
Usada quando temos mais de duas possibilidades lógicas de ramificação. Podemos encadear várias condições sequencialmente. O programa testará cada uma até encontrar a primeira verdadeira, ignorando as demais a partir desse ponto.

**Exemplo:**
```
nota <- 6
SE (nota >= 7) ENTAO
    escreva("Aluno Aprovado")
SENAO SE (nota >= 5) ENTAO
    escreva("Aluno em Recuperação")
SENAO
    escreva("Aluno Reprovado")
FIM SE
```

### 4. Estrutura de Múltipla Escolha (ESCOLHA... CASO / SWITCH... CASE)
Quando precisamos testar o valor exato de uma única variável contra várias opções diferentes (como opções numéricas inteiras ou caracteres), o uso de vários "SE... SENAO SE" pode tornar o código difícil de ler. A estrutura de Múltipla Escolha avalia a variável e direciona a execução para o "caso" correspondente de forma mais elegante.

**Exemplo em Pseudocódigo:**
```
opcao_menu <- 2
ESCOLHA (opcao_menu)
    CASO 1:
        escreva("Você escolheu a Opção 1: Iniciar Jogo")
        PARE
    CASO 2:
        escreva("Você escolheu a Opção 2: Configurações")
        PARE
    CASO 3:
        escreva("Você escolheu a Opção 3: Sair")
        PARE
    CASO PADRAO:
        escreva("Opção Inválida. Tente novamente.")
FIM ESCOLHA
```

## Operadores Essenciais
Para construir as condições dentro das estruturas de decisão, utilizamos dois grupos de operadores:
*   **Operadores Relacionais:** Utilizados para comparar valores. Exemplos: Igual (==), Diferente (!=), Maior que (>), Menor que (<), Maior ou igual (>=), Menor ou igual (<=).
*   **Operadores Lógicos:** Utilizados para combinar múltiplas condições. Exemplos: E (AND - exige que todas as condições conjuntas sejam verdadeiras), OU (OR - basta que pelo menos uma seja verdadeira), NAO (NOT - inverte o resultado lógico).

## Conclusão
As estruturas de decisão são essenciais porque dão a capacidade de adaptação ao programa, permitindo que ele aja e reaja de formas diferentes dependendo dos dados de entrada, de cálculos anteriores ou do estado geral do sistema. Compreendê-las é o requisito fundamental para o desenvolvimento de qualquer software interativo e inteligente.
