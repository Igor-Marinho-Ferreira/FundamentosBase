
# Resolução Exercícios sobre Matrizes em PHP

## Exercício 1: Criação de uma Matriz 2x3
```php
<?php
$matriz = [
    [1, 2, 3],
    [4, 5, 6]
];

for ($i = 0; $i < 2; $i++) {
    for ($j = 0; $j < 3; $j++) {
        echo $matriz[$i][$j] . " ";
    }
    echo "\n";
}
?>
```

## Exercício 2: Soma de Elementos de uma Linha
```php
<?php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

$soma = 0;
for ($j = 0; $j < 3; $j++) {
    $soma += $matriz[0][$j];
}

echo "A soma dos elementos da primeira linha é: $soma\n";
?>
```

## Exercício 3: Maior Elemento de Cada Coluna
```php
<?php
$matriz = [
    [3, 2, 1],
    [6, 5, 4],
    [9, 8, 7]
];

for ($j = 0; $j < 3; $j++) {
    $maior = $matriz[0][$j];
    for ($i = 1; $i < 3; $i++) {
        if ($matriz[$i][$j] > $maior) {
            $maior = $matriz[$i][$j];
        }
    }
    echo "O maior elemento da coluna $j é: $maior\n";
}
?>
```

## Exercício 4: Produto de Matrizes
```php
<?php
$matriz1 = [
    [1, 2],
    [3, 4]
];

$matriz2 = [
    [5, 6],
    [7, 8]
];

$resultado = [
    [0, 0],
    [0, 0]
];

for ($i = 0; $i < 2; $i++) {
    for ($j = 0; $j < 2; $j++) {
        for ($k = 0; $k < 2; $k++) {
            $resultado[$i][$j] += $matriz1[$i][$k] * $matriz2[$k][$j];
        }
    }
}

for ($i = 0; $i < 2; $i++) {
    for ($j = 0; $j < 2; $j++) {
        echo $resultado[$i][$j] . " ";
    }
    echo "\n";
}
?>
```

## Exercício 5: Rotação de uma Matriz 3x3
```php
<?php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

$rotacionada = [
    [0, 0, 0],
    [0, 0, 0],
    [0, 0, 0]
];

for ($i = 0; $i < 3; $i++) {
    for ($j = 0; $j < 3; $j++) {
        $rotacionada[$j][2 - $i] = $matriz[$i][$j];
    }
}

for ($i = 0; $i < 3; $i++) {
    for ($j = 0; $j < 3; $j++) {
        echo $rotacionada[$i][$j] . " ";
    }
    echo "\n";
}
?>
```
