
# Resolução dos exercícios sobre Vetores em PHP

## 1. Criação de Vetor Vazio

```php
<?php
$cidades = [];
$cidades[] = "São Paulo";
$cidades[] = "Rio de Janeiro";
$cidades[] = "Belo Horizonte";

foreach ($cidades as $cidade) {
    echo $cidade . "<br>";
}
?>
```

## 2. Inicialização de Vetor com Números

```php
<?php
$numeros = [1, 2, 3, 4, 5];

foreach ($numeros as $numero) {
    echo $numero . "<br>";
}
?>
```

## 3. Acesso a Elementos do Vetor

```php
<?php
$cores = ["vermelho", "azul", "verde"];
echo $cores[1];
?>
```

## 4. Modificação de Valores no Vetor

```php
<?php
$animais = ["cachorro", "gato", "coelho"];
$animais[1] = "tartaruga";

print_r($animais);
?>
```

## 5. Tamanho do Vetor

```php
<?php
$frutas = ["maçã", "banana", "laranja"];
echo count($frutas);
?>
```

## 6. Soma dos Elementos de um Vetor

```php
<?php
$numeros = [10, 20, 30, 40, 50];
$soma = array_sum($numeros);

echo $soma;
?>
```

## 7. Vetor de Notas

```php
<?php
$notas = [7.5, 8.0, 9.2, 6.8, 7.9];
$media = array_sum($notas) / count($notas);

echo $media;
?>
```

## 8. Encontrar um Elemento em um Vetor

```php
<?php
$alunos = ["Ana", "João", "Maria", "Pedro"];

if (in_array("Maria", $alunos)) {
    echo "Maria está no vetor.";
} else {
    echo "Maria não está no vetor.";
}
?>
```

## 9. Multiplicação dos Elementos de um Vetor

```php
<?php
$fatores = [2, 3, 4, 5];
$produto = array_product($fatores);

echo $produto;
?>
```

## 10. Inverter um Vetor

```php
<?php
$dias = ["segunda", "terça", "quarta", "quinta", "sexta"];
$dias_invertidos = array_reverse($dias);

print_r($dias_invertidos);
?>
```

## 11. Filtragem de Vetor

```php
<?php
$idades = [12, 18, 25, 40, 33, 15];
$idades_filtradas = array_filter($idades, function($idade) {
    return $idade >= 18;
});

print_r($idades_filtradas);
?>
```

## 12. Ordenação de Vetor

```php
<?php
$valores = [45, 12, 78, 34, 23];
sort($valores);

print_r($valores);
?>
```

## 13. Vetor Associativo

```php
<?php
$pessoa = [
    "nome" => "Seu Nome",
    "idade" => 30,
    "cidade" => "Sua Cidade"
];

foreach ($pessoa as $chave => $valor) {
    echo "$chave: $valor<br>";
}
?>
```

## 14. Contagem de Ocorrências em um Vetor

```php
<?php
$palavras = ["casa", "carro", "casa", "bicicleta", "carro", "casa"];
$contagem_casa = array_count_values($palavras)["casa"];

echo $contagem_casa;
?>
```

## 15. Intersecção de Vetores

```php
<?php
$vetor1 = [1, 2, 3, 4, 5];
$vetor2 = [3, 4, 5, 6, 7];
$interseccao = array_intersect($vetor1, $vetor2);

print_r($interseccao);
?>
```
