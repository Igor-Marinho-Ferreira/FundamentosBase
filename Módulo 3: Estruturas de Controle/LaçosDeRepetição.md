# Módulo 3: Estrutura de Controle - Laços de repetição

## Laço de repetição FOR

### Explicação
O laço for é usado quando você sabe exatamente quantas vezes deseja repetir um bloco de código. Ele é composto por três partes: inicialização, condição e incremento.

### Estrutura do laço
```php
for (inicialização; condição; incremento) {
    // Código a ser repetido
}
```
### Exemplo
Imagine que você tem uma caixa de bombons e deseja comer um bombom por dia até acabar. Suponha que a caixa tenha 5 bombons.

### Resolução do exemplo
```php
for ($bombom = 1; $bombom <= 5; $bombom++) {
    echo "Comi o bombom número $bombom<br>";
}
```
### Uso:
- O laço for é ideal quando você sabe de antemão quantas vezes o bloco de código deve ser repetido.
- É frequentemente usado quando há uma necessidade clara de um contador ou índice.

### Quando Usar:
- Para iterar sobre uma sequência de números.
- Para executar um bloco de código um número específico de vezes.

## Laço de repetição FOREACH

### Explicação
O laço foreach é usado para percorrer todos os elementos de um array. Ele é particularmente útil quando você não precisa de um contador, apenas deseja acessar diretamente os elementos do array.

### Estrutura do laço
```php
foreach ($array as $valor) {
    // Código a ser repetido para cada valor do array
}
```
### Exemplo
Imagine que você tem uma lista de frutas para comprar e deseja imprimir cada fruta da lista.

### Resolução do exemplo
```php
$frutas = ["Maçã", "Banana", "Laranja", "Uva"];

foreach ($frutas as $fruta) {
    echo "Preciso comprar $fruta<br>";
}
```
### Uso:
- O laço foreach é projetado especificamente para iterar sobre arrays.
- Não requer um contador ou índice explícito.

### Quando Usar:
- Para percorrer todos os elementos de um array de forma simples e direta.
- Quando você deseja acessar diretamente os valores dos elementos do array.
