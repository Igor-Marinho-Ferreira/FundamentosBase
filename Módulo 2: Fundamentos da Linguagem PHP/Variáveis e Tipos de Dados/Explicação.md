# Módulo 2: Fundamentos da Linguagem PHP - Variáveis e Tipos de Dados

## Explicação
No PHP, os tipos de dados são fundamentais para o armazenamento e manipulação das informações. Os principais tipos de dados incluem inteiros, strings, booleanos e arrays.

## Inteiros

### Explicação
Os inteiros são números sem ponto decimal. Eles podem ser positivos, negativos ou zero.

### Estrutura 
```php
$numero = 123;
```

### Exemplo
```php
$idade = 25;
echo $idade; // Exibe: 25
```

## Strings

### Explicação
As strings são sequências de caracteres, usadas para representar texto.

### Estrutura 
```php
$texto = "Olá, mundo!";
```

### Exemplo
```php
$mensagem = "Bem-vindo ao PHP!";
echo $mensagem; // Exibe: Bem-vindo ao PHP!
```

## Booleanos

### Explicação
Os booleanos representam valores de verdade, sendo true ou false.

### Estrutura 
```php
$verdadeiro = true;
$falso = false;
```

### Exemplo
```php
$isAdmin = true;
if ($isAdmin) {
    echo "Você tem acesso de administrador.";
} else {
    echo "Você não tem acesso de administrador.";
}
```

## Arrays

### Explicação
Os arrays são coleções de valores, onde cada valor é identificado por uma chave. Arrays podem armazenar múltiplos valores em uma única variável.

### Estrutura 
```php
$numeros = [1, 2, 3, 4, 5];
```

### Exemplo
```php
$frutas = ["maçã", "banana", "laranja"];
echo $frutas[1]; // Exibe: banana
```

## Declaração de variáveis e constantes

### Explicação
Variáveis são utilizadas para armazenar dados que podem mudar durante a execução do script, enquanto constantes armazenam valores que não mudam.

## Declaração de Variáveis

### Explicação
Para declarar uma variável no PHP, use o símbolo $ seguido do nome da variável.

### Estrutura 
```php
$nomeVariavel = valor;
```

### Exemplo
```php
$nome = "João";
$idade = 30;
echo "Nome: $nome, Idade: $idade"; // Exibe: Nome: João, Idade: 30
```

## Declaração de Constantes

### Explicação
Constantes são definidas usando a função define() ou a palavra-chave const.

### Estrutura 
```php
define("NOME_CONSTANTE", valor);
const NOME_CONSTANTE = valor;
```

### Exemplo
```php
define("PI", 3.1415926535898);
const TAXA_CAMBIO = 5.17;

echo "Valor de PI: " . PI; // Exibe: Valor de PI: 3.1415926535898
echo "Taxa de Câmbio: " . TAXA_CAMBIO; // Exibe: Taxa de Câmbio: 5.17
```

## Uso
- Inteiros: Quando precisar trabalhar com números inteiros.
- Strings: Quando precisar manipular ou exibir texto.
- Booleanos: Quando precisar trabalhar com condições e lógica.
- Arrays: Quando precisar armazenar múltiplos valores em uma única variável.
- Variáveis: Quando precisar de dados que podem mudar durante a execução do script.
- Constantes: Quando precisar de valores fixos durante toda a execução do script.
