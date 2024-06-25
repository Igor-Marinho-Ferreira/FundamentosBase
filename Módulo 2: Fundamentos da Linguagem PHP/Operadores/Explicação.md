# Módulo 2: Fundamentos da Linguagem PHP - Operadores

## Operadores Aritméticos

### Explicação
Os operadores aritméticos são usados para realizar operações matemáticas.

### Tipos de Operadores Aritméticos
- Adição (+): Soma de dois valores.
- Subtração (-): Subtrai um valor de outro.
- Multiplicação (*): Multiplica dois valores.
- Divisão (/): Divide um valor por outro.
- Módulo (%): Retorna o restante da divisão de um valor por outro.

### Estrutura 
```php
$a + $b;
$a - $b;
$a * $b;
$a / $b;
$a % $b;
```

### Exemplo
```php
$a = 10;
$b = 2;

echo $a + $b; // Exibe: 12
echo $a - $b; // Exibe: 8
echo $a * $b; // Exibe: 20
echo $a / $b; // Exibe: 5
echo $a % $b; // Exibe: 0
```

## Operadores de Comparação

### Explicação
Os operadores de comparação são usados para comparar dois valores.

### Tipos de Operadores de Comparação
- Igual (==): Verifica se dois valores são iguais.
- Idêntico (===): Verifica se dois valores são iguais e do mesmo tipo.
- Diferente (!=): Verifica se dois valores são diferentes.
- Não idêntico (!==): Verifica se dois valores são diferentes ou não são do mesmo tipo.
- Menor que (<): Verifica se um valor é menor que outro.
- Maior que (>): Verifica se um valor é maior que outro.
- Menor ou igual (<=): Verifica se um valor é menor ou igual a outro.
- Maior ou igual (>=): Verifica se um valor é maior ou igual a outro.
    
### Estrutura 
```php
$a == $b;
$a === $b;
$a != $b;
$a !== $b;
$a < $b;
$a > $b;
$a <= $b;
$a >= $b;
```

### Exemplo
```php
$a = 5;
$b = 10;

echo $a == $b; // Exibe: false
echo $a < $b; // Exibe: true
```

## Operadores Lógicos

### Explicação
Os operadores lógicos são usados para combinar múltiplas expressões condicionais.

### Tipos de Operadores Lógicos

- E (&&): Retorna true se ambas as expressões forem verdadeiras.
- Ou (||): Retorna true se pelo menos uma das expressões for verdadeira.
- Não (!): Inverte o valor lógico de uma expressão.
    
### Estrutura 
```php
$a && $b;
$a || $b;
!$a;
```

### Exemplo
```php
$a = true;
$b = false;

echo $a && $b; // Exibe: false
echo $a || $b; // Exibe: true
echo !$a; // Exibe: false
```

## Operadores de Atribuição

### Explicação
Os operadores de atribuição são usados para atribuir valores às variáveis.

### Tipos de Operadores de Atribuição

- Atribuição Simples (=): Atribui um valor a uma variável.
- Atribuição com Adição (+=): Adiciona um valor à variável e atribui o resultado à variável.
- Atribuição com Subtração (-=): Subtrai um valor da variável e atribui o resultado à variável.
- Atribuição com Multiplicação (*=): Multiplica a variável por um valor e atribui o resultado à variável.
- Atribuição com Divisão (/=): Divide a variável por um valor e atribui o resultado à variável.
    
### Estrutura 
```php
$a = $b;
$a += $b;
$a -= $b;
$a *= $b;
$a /= $b;
```

### Exemplo
```php
$a = 10;
$b = 5;

$a += $b; // $a agora é 15
echo $a; // Exibe: 15
```

## Operadores de Concatenação

### Explicação
Os operadores de concatenação são usados para unir strings.

### Tipos de Operadores de Concatenação
- Concatenação (.): Une duas strings.
- Concatenação e Atribuição (.=): Concatena uma string à variável e atribui o resultado à variável.
    
### Estrutura 
```php
$a . $b;
$a .= $b;
```

### Exemplo
```php
$a = "Olá, ";
$b = "mundo!";

echo $a . $b; // Exibe: Olá, mundo!

$a .= $b; // $a agora é "Olá, mundo!"
echo $a; // Exibe: Olá, mundo!
```

## Uso
- Operadores Aritméticos: Quando precisar realizar cálculos matemáticos.
- Operadores de Comparação: Quando precisar comparar valores.
- Operadores Lógicos: Quando precisar combinar múltiplas condições.
- Operadores de Atribuição: Quando precisar atribuir ou atualizar valores de variáveis.
- Operadores de Concatenação: Quando precisar unir strings.
