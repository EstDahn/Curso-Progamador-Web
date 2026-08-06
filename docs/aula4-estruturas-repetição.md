# Aula 4: Estruturas de Repetição na Lógica de Programação

## Introdução
Na programação, muitas vezes precisamos executar o mesmo bloco de código várias vezes. Escrever as mesmas instruções repetidamente torna o código longo, difícil de ler e propenso a erros. Para resolver esse problema, utilizamos as **Estruturas de Repetição** (também conhecidas como loops ou laços).

As estruturas de repetição permitem que um conjunto de instruções seja executado repetidamente enquanto uma determinada condição for verdadeira ou até que um número específico de iterações seja alcançado.

## Principais Estruturas de Repetição

Existem três tipos principais de estruturas de repetição que encontramos na maioria das linguagens de programação e em pseudocódigos:

### 1. Estrutura ENQUANTO (While)
A estrutura `ENQUANTO` verifica a condição **antes** de executar o bloco de código. Se a condição for verdadeira, o código é executado. Esse ciclo se repete até que a condição se torne falsa. Se a condição for falsa logo no início, o código dentro do laço nunca será executado.

**Quando usar:** Quando não sabemos exatamente quantas vezes o bloco precisará ser repetido, mas sabemos a condição que deve parar a repetição.

**Exemplo em Pseudocódigo:**
```
inteiro contador <- 1
enquanto (contador <= 5) faca
    escreva("Esta é a repetição número: ", contador)
    contador <- contador + 1
fimenquanto
```

### 2. Estrutura PARA (For)
A estrutura `PARA` é utilizada quando sabemos de antemão exatamente quantas vezes o bloco de código deve ser repetido. Ela geralmente inicializa uma variável de controle, define a condição de parada e o incremento (ou decremento) em uma única linha de instrução.

**Quando usar:** Quando o número exato de iterações é conhecido ou quando precisamos percorrer elementos de uma lista, ou vetor.

**Exemplo em Pseudocódigo:**
```
para contador de 1 ate 5 passo 1 faca
    escreva("Esta é a repetição número: ", contador)
fimpara
```

### 3. Estrutura REPITA... ATE (Do-While / Repeat-Until)
A estrutura `REPITA` executa o bloco de código primeiro e verifica a condição de parada **depois**. Isso garante que o código dentro do laço seja executado pelo menos uma vez, mesmo que a condição de parada já seja verdadeira na primeira verificação.

**Quando usar:** Quando o bloco de código precisa ser executado obrigatoriamente pelo menos uma vez (por exemplo, na leitura e validação de uma entrada de usuário).

**Exemplo em Pseudocódigo:**
```
inteiro senha
repita
    escreva("Digite a senha:")
    leia(senha)
ate (senha == 1234)
escreva("Acesso permitido.")
```

## O Perigo dos Loops Infinitos
Um conceito crítico nas estruturas de repetição é a garantia de que a condição de parada será atingida em algum momento. Se a variável que controla o laço nunca for atualizada ou a condição lógica estiver incorreta, o programa continuará executando o bloco de código para sempre. Isso é chamado de **Loop Infinito** e geralmente causa o travamento do programa ou exaustão de memória.

**Exemplo de Loop Infinito (Incorreto):**
```
inteiro x <- 1
enquanto (x < 10) faca
    escreva("O valor de x é: ", x)
    // Erro: esquecemos de incrementar o x. A condição (x < 10) será sempre verdadeira.
fimenquanto
```

## Conclusão
Dominar as estruturas de repetição é fundamental para criar algoritmos eficientes e dinâmicos. A escolha entre `ENQUANTO`, `PARA` ou `REPITA` depende do problema específico que você está tentando resolver, especialmente se o número de repetições é previamente conhecido e o momento em que a condição de parada deve ser testada.
