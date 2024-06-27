### Resolução dos exercícios de laço de repetição

## Laço de Repetição for

1. Escreva um for que exiba os números de 1 a 10.
```php
for ($i = 1; $i <= 10; $i++) {
    echo $i . "\n";
}
```
2. Crie um for que imprima os números pares de 2 a 20.
```php
for ($i = 2; $i <= 20; $i += 2) {
    echo $i . "\n";
}
```
3. Implemente um for que conte de 10 até 1, exibindo cada número.
```php
for ($i = 10; $i >= 1; $i--) {
    echo $i . "\n";
}
```
4. Escreva um for que calcule a soma dos números de 1 a 100 e exiba o resultado.
```php
$soma = 0;
for ($i = 1; $i <= 100; $i++) {
    $soma += $i;
}
echo "Soma dos números de 1 a 100: " . $soma . "\n";
```
5. Implemente um for que itere sobre uma lista de números e calcule a média dos valores.
```php
$numeros = [1, 2, 3, 4, 5];
$soma = 0;
for ($i = 0; $i < count($numeros); $i++) {
    $soma += $numeros[$i];
}
$media = $soma / count($numeros);
echo "Média dos valores: " . $media . "\n";
```

## Laço de Repetição foreach

1. Utilize um foreach para imprimir cada elemento de uma lista de cores (ex: vermelho, azul, verde).
```php
$cores = ["vermelho", "azul", "verde"];
foreach ($cores as $cor) {
    echo $cor . "\n";
}
```
2. Itere sobre um array de nomes de frutas utilizando foreach e exiba cada fruta.
```php
$frutas = ["maçã", "banana", "laranja"];
foreach ($frutas as $fruta) {
    echo $fruta . "\n";
}
```
3. Crie um foreach que some os valores de um array numérico e exiba o resultado.
```php
$numeros = [1, 2, 3, 4, 5];
$soma = 0;
foreach ($numeros as $numero) {
    $soma += $numero;
}
echo "Soma dos valores: " . $soma . "\n";
```
4. Utilize um foreach para calcular e exibir a multiplicação de todos os elementos de um array numérico.
```php
$numeros = [1, 2, 3, 4, 5];
$produto = 1;
foreach ($numeros as $numero) {
    $produto *= $numero;
}
echo "Multiplicação dos valores: " . $produto . "\n";
```
5. Implemente um foreach que identifique e exiba o maior número em um array numérico.
```php
$numeros = [1, 2, 3, 4, 5];
$maior = $numeros[0];
foreach ($numeros as $numero) {
    if ($numero > $maior) {
        $maior = $numero;
    }
}
echo "Maior número: " . $maior . "\n";
```

## Laço de Repetição while

1. Escreva um while que conte de 1 a 5 e exiba cada número.
```php
$i = 1;
while ($i <= 5) {
    echo $i . "\n";
    $i++;
}
```
2. Implemente um while que imprima os números pares de 1 a 10.
```php
$i = 1;
while ($i <= 10) {
    if ($i % 2 == 0) {
        echo $i . "\n";
    }
    $i++;
}
```
3. Utilize um while para exibir a tabuada do 5 (de 1 a 10).
```php
$i = 1;
while ($i <= 10) {
    echo "5 x " . $i . " = " . (5 * $i) . "\n";
    $i++;
}
```
4. Escreva um while que calcule e exiba a média de uma lista de números fornecidos pelo usuário.
```php
$numeros = [10, 20, 30, 40, 50]; // Lista de números pré-definidos
$soma = 0;
$contador = count($numeros);
$indice = 0;

while ($indice < $contador) {
    $soma += $numeros[$indice];
    $indice++;
}

$media = $soma / $contador;
echo "Média dos valores: " . $media . "\n";
```

5. Implemente um while que leia números do usuário até que um número negativo seja digitado, calcule e exiba a soma dos números positivos digitados.
```php
$numeros = [5, 10, 15, -5, 20, 25]; // Lista de números pré-definidos
$soma = 0;
$indice = 0;

while ($indice < count($numeros) && $numeros[$indice] >= 0) {
    $soma += $numeros[$indice];
    $indice++;
}

echo "Soma dos números positivos: " . $soma . "\n";
```
