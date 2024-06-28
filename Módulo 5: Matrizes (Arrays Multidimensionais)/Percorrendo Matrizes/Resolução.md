# Resolução Matrizes (Arrays Multidimensionais) - Percorrendo Matrizes

### Exercício 1: Percorrendo uma Matriz com `for`

Escreva um script PHP que percorra uma matriz 2x3 e exiba cada elemento com sua respectiva posição.

### Instruções: 
1. Crie uma matriz: `$matriz = [[1, 2, 3], [4, 5, 6]]`.
2. Utilize laços aninhados `for` para percorrer a matriz.
3. Exiba cada elemento com sua respectiva posição.

### Solução:
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6]
];

for ($i = 0; $i < count($matriz); $i++) {
    for ($j = 0; $j < count($matriz[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $matriz[$i][$j] . "<br>";
    }
}
```

### Exercício 2: Percorrendo uma Matriz com `foreach`

Escreva um script PHP que percorra uma matriz de categorias de frutas e exiba cada fruta.

### Instruções:
1. Crie uma matriz: `$frutas = [["Maçã", "Banana"], ["Morango", "Uva"], ["Abacaxi", "Manga"]]`.
2. Utilize laços aninhados `foreach` para percorrer a matriz.
3. Exiba cada fruta.

### Solução:
```php
$frutas = [
    ["Maçã", "Banana"],
    ["Morango", "Uva"],
    ["Abacaxi", "Manga"]
];

foreach ($frutas as $categoria) {
    foreach ($categoria as $fruta) {
        echo "Fruta: " . $fruta . "<br>";
    }
}
```

### Exercício 3: Percorrendo uma Matriz e Somando os Elementos

Escreva um script PHP que percorra uma matriz 3x3 de números e calcule a soma de todos os elementos.

### nstruções:
1. Crie uma matriz: `$numeros = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]`.
2. Utilize laços aninhados `for` para percorrer a matriz.
3. Calcule e exiba a soma de todos os elementos.

### Solução:
```php
$numeros = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
$soma = 0;

for ($i = 0; $i < count($numeros); $i++) {
    for ($j = 0; $j < count($numeros[$i]); $j++) {
        $soma += $numeros[$i][$j];
    }
}

echo "Soma de todos os elementos: " . $soma;
```

### Exercício 4: Percorrendo uma Matriz e Encontrando o Maior Elemento

Escreva um script PHP que percorra uma matriz 3x3 de números e encontre o maior elemento.

### Instruções:
1. Crie uma matriz: `$numeros = [[3, 5, 1], [7, 8, 2], [4, 6, 9]]`.
2. Utilize laços aninhados `foreach` para percorrer a matriz.
3. Encontre e exiba o maior elemento.

### Solução:
```php
$numeros = [
    [3, 5, 1],
    [7, 8, 2],
    [4, 6, 9]
];
$maior = $numeros[0][0];

foreach ($numeros as $linha) {
    foreach ($linha as $numero) {
        if ($numero > $maior) {
            $maior = $numero;
        }
    }
}

echo "O maior elemento é: " . $maior;
```

### Exercício 5: Manipulação Complexa de Matrizes

Escreva um script PHP que percorra uma matriz 4x4 de números, inverta a ordem dos elementos de cada linha e exiba a matriz resultante.

### Instruções:
1. Crie uma matriz: `$numeros = [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]]`.
2. Utilize laços aninhados `for` para percorrer a matriz.
3. Inverta a ordem dos elementos de cada linha.
4. Exiba a matriz resultante.

### Solução:
```php
$numeros = [
    [1, 2, 3, 4],
    [5, 6, 7, 8],
    [9, 10, 11, 12],
    [13, 14, 15, 16]
];

for ($i = 0; $i < count($numeros); $i++) {
    $numeros[$i] = array_reverse($numeros[$i]);
}

for ($i = 0; $i < count($numeros); $i++) {
    for ($j = 0; $j < count($numeros[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $numeros[$i][$j] . "<br>";
    }
}
```
