# Módulo 3: Estrutura de Controle - Estrutura de decisão

## if statement (se):

### Explicação
A estrutura if é fundamental na programação para executar um bloco de código se uma condição especificada for verdadeira.

### Estrutura 
```php
if (condição) {
    // bloco de código a ser executado se a condição for verdadeira
}
```
### Exemplo
Imagine um sistema de verificação de idade para acesso a determinados conteúdos online:

### Resolução do exemplo
```php
$idade = 20;

if ($idade >= 18) {
    echo "Você tem permissão para acessar o conteúdo para maiores de idade.";
}
```
### Uso:
- Quando usar: Utilize if quando precisar executar um bloco de código se uma condição for verdadeira.

## else if statement (senão, se):

### Explicação
A estrutura elseif é usada para adicionar mais condições à estrutura if. Ela verifica condições adicionais se a primeira condição do if for falsa.

### Estrutura
```php
if (condição1) {
    // bloco de código a ser executado se a condição1 for verdadeira
} elseif (condição2) {
    // bloco de código a ser executado se a condição2 for verdadeira
}

```
### Exemplo
Vamos estender o exemplo anterior para incluir uma condição adicional para adolescentes:

### Resolução do exemplo
```php
$idade = 15;

if ($idade >= 18) {
    echo "Você tem permissão para acessar o conteúdo para maiores de idade.";
} elseif ($idade >= 13) {
    echo "Você tem permissão para acessar o conteúdo para adolescentes.";
}
```
### Uso:
- Quando usar: Use elseif para verificar condições adicionais se a condição do if não for verdadeira.

## else statement (senão)

### Explicação
A estrutura else é usada para executar um bloco de código se a condição do if for falsa. É a última opção dentro de uma estrutura condicional.

### Estrutura
```php
if (condição) {
    // bloco de código a ser executado se a condição for verdadeira
} else {
    // bloco de código a ser executado se a condição for falsa
}
```
### Exemplo
Agora, vamos expandir nosso exemplo para incluir uma mensagem para menores de 13 anos:

### Resolução do exemplo
```php
$idade = 10;

if ($idade >= 18) {
    echo "Você tem permissão para acessar o conteúdo para maiores de idade.";
} elseif ($idade >= 13) {
    echo "Você tem permissão para acessar o conteúdo para adolescentes.";
} else {
    echo "Desculpe, você não tem permissão para acessar este conteúdo.";
}

```
### Uso:
- Quando usar: Use else para tratar qualquer outra condição que não tenha sido coberta pelas verificações anteriores.
