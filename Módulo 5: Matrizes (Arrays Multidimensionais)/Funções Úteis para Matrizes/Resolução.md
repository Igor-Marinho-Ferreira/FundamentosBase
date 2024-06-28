
# Resolução Matrizes (Arrays Multidimensionais) - Funções Úteis para Matrizes

### Exercício 1: Combinando Arrays com `array_merge()`

Escreva um script PHP que combine dois arrays de frutas e exiba o resultado.

### Instruções:
1. Crie dois arrays: `$frutas1 = ['Maçã', 'Banana', 'Cereja']` e `$frutas2 = ['Laranja', 'Manga', 'Uva']`.
2. Utilize a função `array_merge()` para combinar os arrays.
3. Exiba o array combinado.

### Solução:
```php
$frutas1 = ['Maçã', 'Banana', 'Cereja'];
$frutas2 = ['Laranja', 'Manga', 'Uva'];
$frutasCombinadas = array_merge($frutas1, $frutas2);

foreach ($frutasCombinadas as $fruta) {
    echo "Fruta: " . $fruta . "<br>";
}
```

### Exercício 2: Extraindo Chaves com `array_keys()`

Escreva um script PHP que extraia e exiba todas as chaves de um array associativo de carros.

### Instruções:
1. Crie um array associativo: `$carros = ['BMW' => 'X5', 'Audi' => 'A4', 'Toyota' => 'Corolla']`.
2. Utilize a função `array_keys()` para obter as chaves do array.
3. Exiba as chaves.

### Solução:
```php
$carros = ['BMW' => 'X5', 'Audi' => 'A4', 'Toyota' => 'Corolla'];
$chaves = array_keys($carros);

foreach ($chaves as $chave) {
    echo "Marca: " . $chave . "<br>";
}
```
### Exercício 3: Extraindo Valores com `array_values()`

Escreva um script PHP que extraia e exiba todos os valores de um array associativo de livros.

### Instruções:
1. Crie um array associativo: `$livros = ['Autor1' => 'Livro1', 'Autor2' => 'Livro2', 'Autor3' => 'Livro3']`.
2. Utilize a função `array_values()` para obter os valores do array.
3. Exiba os valores.

### Solução:
```php
$livros = ['Autor1' => 'Livro1', 'Autor2' => 'Livro2', 'Autor3' => 'Livro3'];
$valores = array_values($livros);

foreach ($valores as $valor) {
    echo "Livro: " . $valor . "<br>";
}
```

### Exercício 4: Conversão de Vetor para Matriz

Escreva um script PHP que converta um vetor de números em uma matriz de 3x2.

### Instruções:
1. Crie um vetor: `$numeros = [1, 2, 3, 4, 5, 6]`.
2. Utilize a função `array_chunk()` para converter o vetor em uma matriz de 3x2.
3. Exiba a matriz.

### Solução:
```php
$numeros = [1, 2, 3, 4, 5, 6];
$matriz = array_chunk($numeros, 2);

foreach ($matriz as $linha) {
    foreach ($linha as $elemento) {
        echo "Elemento: " . $elemento . "<br>";
    }
}
```

### Exercício 5: Conversão de Matriz para Vetor e Manipulação

Escreva um script PHP que converta uma matriz 2x2 em um vetor, depois combine este vetor com outro vetor de números e exiba o resultado.

### Instruções:
1. Crie uma matriz: `$matriz = [[7, 8], [9, 10]]`.
2. Converta a matriz em um vetor utilizando `array_merge()`.
3. Crie um segundo vetor: `$outrosNumeros = [11, 12, 13]`.
4. Combine os vetores utilizando `array_merge()`.
5. Exiba o vetor combinado.

### Solução:
```php
$matriz = [[7, 8], [9, 10]];
$vetor = array_merge(...$matriz);

$outrosNumeros = [11, 12, 13];
$vetorCombinado = array_merge($vetor, $outrosNumeros);

foreach ($vetorCombinado as $numero) {
    echo "Número: " . $numero . "<br>";
}
```
