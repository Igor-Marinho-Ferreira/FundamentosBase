### Exercícios de Estrutura de decisão

## if

1. Verifique se um número é positivo.
```php
$numero = 10;
if ($numero > 0) {
    echo "$numero é positivo.";
}
```
2. Verifique se uma pessoa é maior de idade.
```php
$idade = 20;
if ($idade >= 18) {
    echo "A pessoa é maior de idade.";
}
```
3. Verifique se um número é par.
```php
$numero = 4;
if ($numero % 2 == 0) {
    echo "$numero é par.";
}
```
4. Verifique se uma string contém outra.
```php
$string1 = "Olá, mundo!";
$string2 = "mundo";
if (strpos($string1, $string2) !== false) {
    echo "A string contém a outra.";
}
```
5. Verifique se um ano é bissexto.
```php
$ano = 2020;
if (($ano % 4 == 0 && $ano % 100 != 0) || ($ano % 400 == 0)) {
    echo "$ano é bissexto.";
}
```

## elseif

1. Verifique se um número é positivo, negativo ou zero.
```php
$numero = -5;
if ($numero > 0) {
    echo "$numero é positivo.";
} elseif ($numero < 0) {
    echo "$numero é negativo.";
} else {
    echo "$numero é zero.";
}
```
2. Verifique se um aluno passou ou reprovou.
```php
$nota = 7.5;
$media = 6.0;
if ($nota >= $media) {
    echo "O aluno passou.";
} else {
    echo "O aluno reprovou.";
}
```
3. Verifique a faixa etária de uma pessoa.
```php
$idade = 25;
if ($idade < 12) {
    echo "Criança.";
} elseif ($idade < 18) {
    echo "Adolescente.";
} elseif ($idade < 60) {
    echo "Adulto.";
} else {
    echo "Idoso.";
}
```
4. Verifique a categoria de um produto com base no preço.
```php
$preco = 150;
if ($preco < 50) {
    echo "Categoria: Barato.";
} elseif ($preco <= 100) {
    echo "Categoria: Médio.";
} else {
    echo "Categoria: Caro.";
}
```
5. Calcule o imposto de renda baseado em faixas de renda.
```php
$renda = 3000;
if ($renda <= 1903.98) {
    echo "Isento.";
} elseif ($renda <= 2826.65) {
    echo "Imposto de 7.5%.";
} elseif ($renda <= 3751.05) {
    echo "Imposto de 15%.";
} elseif ($renda <= 4664.68) {
    echo "Imposto de 22.5%.";
} else {
    echo "Imposto de 27.5%.";
}
```

## else

1. Verifique se um número é ímpar.
```php
$numero = 7;
if ($numero % 2 == 0) {
    echo "$numero é par.";
} else {
    echo "$numero é ímpar.";
}
```
2. Verifique se uma pessoa pode votar.
```php
$idade = 16;
if ($idade >= 18) {
    echo "A pessoa pode votar.";
} else {
    echo "A pessoa não pode votar.";
}
```
3. Verifique se um número é múltiplo de 5.
```php
$numero = 15;
if ($numero % 5 == 0) {
    echo "$numero é múltiplo de 5.";
} else {
    echo "$numero não é múltiplo de 5.";
}
```
4. Verifique se uma pessoa pode se aposentar.
```php
$idade = 65;
$anosContribuicao = 35;
if ($idade >= 65 && $anosContribuicao >= 30) {
    echo "A pessoa pode se aposentar.";
} else {
    echo "A pessoa não pode se aposentar.";
}
```
5. Verifique se um número está dentro de um intervalo.
```php
$numero = 25;
$minimo = 10;
$maximo = 50;
if ($numero >= $minimo && $numero <= $maximo) {
    echo "$numero está dentro do intervalo.";
} else {
    echo "$numero está fora do intervalo.";
}
```
