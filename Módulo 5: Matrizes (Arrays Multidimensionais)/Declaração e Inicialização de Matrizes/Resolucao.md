
# Resolucao exercícios sobre Matrizes em PHP

## Exercício 1: Criação de uma Matriz 2x2

```php
<?php
// Criação da matriz 2x2
$matriz2x2 = [
    [1, 2],
    [3, 4]
];

// Impressão dos elementos da matriz usando um loop for
for ($i = 0; $i < 2; $i++) {
    for ($j = 0; $j < 2; $j++) {
        echo "Elemento [$i][$j]: " . $matriz2x2[$i][$j] . "<br>";
    }
}
?>
```

## Exercício 2: Criação de uma Matriz 3x1

```php
<?php
// Criação da matriz 3x1
$matriz3x1 = [
    [5],
    [10],
    [15]
];

// Impressão dos elementos da matriz
for ($i = 0; $i < 3; $i++) {
    echo "Elemento [$i][0]: " . $matriz3x1[$i][0] . "<br>";
}
?>
```

## Exercício 3: Matriz 3x3 com Valores Pré-definidos

```php
<?php
// Criação da matriz 3x3
$matriz3x3 = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

// Impressão dos elementos e soma dos valores
$soma = 0;
for ($i = 0; $i < 3; $i++) {
    for ($j = 0; $j < 3; $j++) {
        echo "Elemento [$i][$j]: " . $matriz3x3[$i][$j] . "<br>";
        $soma += $matriz3x3[$i][$j];
    }
}
echo "Soma dos elementos: $soma";
?>
```

## Exercício 4: Matriz de Strings

```php
<?php
// Criação da matriz 2x2 de strings
$matrizStrings = [
    ["Hello", "World"],
    ["PHP", "Matrix"]
];

// Impressão dos elementos da matriz, indicando a posição
for ($i = 0; $i < 2; $i++) {
    for ($j = 0; $j < 2; $j++) {
        echo "Elemento [$i][$j]: " . $matrizStrings[$i][$j] . "<br>";
    }
}
?>
```

## Exercício 5: Transposta de uma Matriz 3x3

```php
<?php
// Criação da matriz 3x3
$matrizOriginal = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

// Criação da matriz transposta
$matrizTransposta = [];
for ($i = 0; $i < 3; $i++) {
    for ($j = 0; $j < 3; $j++) {
        $matrizTransposta[$j][$i] = $matrizOriginal[$i][$j];
    }
}

// Impressão das matrizes original e transposta
echo "Matriz Original:<br>";
for ($i = 0; $i < 3; $i++) {
    for ($j = 0; $j < 3; $j++) {
        echo $matrizOriginal[$i][$j] . " ";
    }
    echo "<br>";
}

echo "Matriz Transposta:<br>";
for ($i = 0; $i < 3; $i++) {
    for ($j = 0; $j < 3; $j++) {
        echo $matrizTransposta[$i][$j] . " ";
    }
    echo "<br>";
}
?>
```
