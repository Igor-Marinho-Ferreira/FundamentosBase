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


## Laço de repetição WHILE

### Explicação
O laço while repete um bloco de código enquanto uma condição for verdadeira. Ele é útil quando você não sabe exatamente quantas vezes precisa repetir o bloco de código, mas sabe a condição que deve ser satisfeita.

### Estrutura do laço
```php
while (condição) {
    // Código a ser repetido
}
```
### Exemplo
Imagine que você está enchendo um balde com água e deseja parar quando o balde estiver cheio. Suponha que o balde tem capacidade para 10 litros.

### Resolução do exemplo
```php
$litros = 0;

while ($litros < 10) {
    $litros++;
    echo "Enchi o balde com mais 1 litro de água. Agora tem $litros litros<br>";
}
```
### Uso:
- O laço while é usado quando você não sabe de antemão quantas vezes o bloco de código deve ser repetido.
- Continua a executar o bloco de código enquanto a condição for verdadeira.

### Quando Usar:
- Para repetir um bloco de código até que uma condição específica seja satisfeita.
- Quando o número de iterações não é conhecido antecipadamente.

## Resumo das Diferenças

### Controle e Estrutura:
- for oferece controle total sobre a inicialização, condição de término e incremento em uma única linha.
- foreach simplifica a iteração sobre arrays, focando nos elementos do array sem a necessidade de um índice.
- while é flexível e adequado para situações onde a repetição depende de uma condição dinâmica.

### Simplicidade e Legibilidade:
- for pode ser mais verboso, mas é claro quando você precisa de um contador.
- foreach é mais legível e conciso para operações com arrays.
- while é claro e direto para condições de repetição indefinidas.

### Uso Comum:
- Use for quando souber o número exato de iterações.
- Use foreach quando trabalhar com arrays e quiser simplicidade.
- Use while quando a repetição depender de uma condição que pode mudar dinamicamente.
