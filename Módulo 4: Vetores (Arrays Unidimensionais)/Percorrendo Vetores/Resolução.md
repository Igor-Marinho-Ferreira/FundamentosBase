
# Resolução dos Exercícios sobre Vetores em PHP

## Exercício 1: Encontrando o Maior e o Menor Valor

```php
<?php
// Criando o vetor com 10 números inteiros aleatórios
$vetor = [];
for ($i = 0; $i < 10; $i++) {
    $vetor[] = rand(1, 100);
}

// Inicializando as variáveis para maior e menor valor
$maior = $vetor[0];
$menor = $vetor[0];

// Percorrendo o vetor para encontrar o maior e o menor valor
for ($i = 1; $i < count($vetor); $i++) {
    if ($vetor[$i] > $maior) {
        $maior = $vetor[$i];
    }
    if ($vetor[$i] < $menor) {
        $menor = $vetor[$i];
    }
}

// Imprimindo os valores
echo "Maior valor: $maior\n";
echo "Menor valor: $menor\n";
?>
```

## Exercício 2: Contagem de Elementos Pares e Ímpares

```php
<?php
// Exemplo de vetor de números inteiros
$vetor = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Inicializando contadores de pares e ímpares
$pares = 0;
$impares = 0;

// Percorrendo o vetor para contar elementos pares e ímpares
foreach ($vetor as $numero) {
    if ($numero % 2 == 0) {
        $pares++;
    } else {
        $impares++;
    }
}

// Imprimindo as quantidades
echo "Quantidade de números pares: $pares\n";
echo "Quantidade de números ímpares: $impares\n";
?>
```

## Exercício 3: Calculando a Média dos Valores

```php
<?php
// Criando o vetor com 15 números inteiros
$vetor = [];
for ($i = 0; $i < 15; $i++) {
    $vetor[] = rand(1, 100);
}

// Calculando a soma dos valores
$soma = 0;
for ($i = 0; $i < count($vetor); $i++) {
    $soma += $vetor[$i];
}

// Calculando a média
$media = $soma / count($vetor);

// Imprimindo a média
echo "Média dos valores: $media\n";
?>
```

## Exercício 4: Vetor de Palíndromos

```php
<?php
// Exemplo de vetor de strings
$vetor = ["radar", "level", "world", "deified", "hello"];

// Função para verificar se uma string é um palíndromo
function isPalindrome($string) {
    $string = strtolower($string);
    return $string == strrev($string);
}

// Verificando e imprimindo as strings que são palíndromos
foreach ($vetor as $palavra) {
    if (isPalindrome($palavra)) {
        echo "$palavra é um palíndromo\n";
    }
}
?>
```

## Exercício 5: Revertendo a Ordem dos Elementos

```php
<?php
// Criando um vetor de números inteiros com 10 elementos
$vetor = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Imprimindo o vetor original
echo "Vetor original: ";
foreach ($vetor as $numero) {
    echo "$numero ";
}
echo "\n";

// Revertendo a ordem dos elementos
$vetorRevertido = [];
for ($i = count($vetor) - 1; $i >= 0; $i--) {
    $vetorRevertido[] = $vetor[$i];
}

// Imprimindo o vetor com a ordem revertida
echo "Vetor revertido: ";
foreach ($vetorRevertido as $numero) {
    echo "$numero ";
}
echo "\n";
?>
```
