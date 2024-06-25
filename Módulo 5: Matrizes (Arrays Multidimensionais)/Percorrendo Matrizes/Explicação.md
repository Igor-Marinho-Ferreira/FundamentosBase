# Módulo 5: Matrizes (Arrays Multidimensionais) - Percorrendo Matrizes

### Uso de Laços Aninhados for para Percorrer Matrizes

### Explicação
Para percorrer uma matriz, utilizamos laços aninhados. O laço externo itera sobre as linhas da matriz, enquanto o laço interno itera sobre as colunas de cada linha. Esta abordagem permite acessar cada elemento da matriz de forma sequencial.

### Estrutura do Laço Aninhado for
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

for ($i = 0; $i < count($matriz); $i++) {
    for ($j = 0; $j < count($matriz[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $matriz[$i][$j] . "<br>";
    }
}
```

### Exemplo
Imagine que você deseja percorrer uma matriz 3x3 e imprimir cada elemento com sua respectiva posição.

### Resolução do Exemplo
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

for ($i = 0; $i < count($matriz); $i++) {
    for ($j = 0; $j < count($matriz[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $matriz[$i][$j] . "<br>";
    }
}
```

### Uso do Laço foreach em Matrizes Multidimensionais

### Explicação
O laço `foreach` pode ser utilizado para percorrer matrizes de forma mais simples e intuitiva. O laço externo percorre cada linha da matriz, enquanto o laço interno percorre cada elemento dentro dessa linha.

### Estrutura do Laço foreach
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];

foreach ($matriz as $linha) {
    foreach ($linha as $elemento) {
        echo "Elemento: " . $elemento . "<br>";
    }
}
```

### Exemplo
Imagine que você deseja percorrer uma matriz de frutas, onde cada linha representa uma categoria de frutas, e imprimir cada fruta.

### Resolução do Exemplo
```php
$frutas = [
    ["Maçã", "Banana", "Laranja"],
    ["Morango", "Uva", "Pêssego"],
    ["Abacaxi", "Manga", "Coco"]
];

foreach ($frutas as $categoria) {
    foreach ($categoria as $fruta) {
        echo "Fruta: " . $fruta . "<br>";
    }
}
```

### Utilidade dos Laços de Repetição
- Laço for: Proporciona controle total sobre os índices e é útil quando você precisa manipular elementos em posições específicas.
- Laço foreach: Simplifica a iteração sobre matrizes, tornando o código mais legível e menos propenso a erros.

### Quando Usar Cada Laço
- Laço for: Utilize quando precisar de controle detalhado sobre os índices e a lógica da iteração.
- Laço foreach: Utilize quando desejar percorrer todos os elementos de uma matriz de forma simples e direta, sem a necessidade de manipular índices.
