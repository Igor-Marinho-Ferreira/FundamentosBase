# Módulo 5: Matrizes (Arrays Multidimensionais) - Funções Úteis para Matrizes

### Funções como array_merge(), array_keys(), array_values()

### Explicação
PHP oferece diversas funções nativas que facilitam a manipulação de matrizes. Estas funções permitem combinar, extrair chaves e valores, e converter entre vetores e matrizes de forma eficiente.

### array_merge()
A função `array_merge()` combina dois ou mais arrays em um único array.

### Estrutura do array_merge()
```php
$array1 = [1, 2, 3];
$array2 = [4, 5, 6];
$resultado = array_merge($array1, $array2);
// Resultado: [1, 2, 3, 4, 5, 6]
```

### Exemplo
Imagine que você deseja combinar duas listas de números em uma única lista.

### Resolução do Exemplo
```php
$lista1 = [1, 2, 3];
$lista2 = [4, 5, 6];
$combinada = array_merge($lista1, $lista2);

foreach ($combinada as $numero) {
    echo "Número: " . $numero . "<br>";
}
```

### array_keys()
A função `array_keys()` retorna todas as chaves de um array.

### Estrutura do array_keys()
```php
$array = [
    "a" => 1,
    "b" => 2,
    "c" => 3
];
$chaves = array_keys($array);
// Resultado: ["a", "b", "c"]
```

### Exemplo
Imagine que você deseja obter todas as chaves de um array associativo.

### Resolução do Exemplo
```php
$array = [
    "a" => 1,
    "b" => 2,
    "c" => 3
];
$chaves = array_keys($array);

foreach ($chaves as $chave) {
    echo "Chave: " . $chave . "<br>";
}
```

### array_values()
A função `array_values()` retorna todos os valores de um array.

### Estrutura do array_values()
```php
$array = [
    "a" => 1,
    "b" => 2,
    "c" => 3
];
$valores = array_values($array);
// Resultado: [1, 2, 3]
```

### Exemplo
Imagine que você deseja obter todos os valores de um array associativo.

### Resolução do Exemplo
```php
$array = [
    "a" => 1,
    "b" => 2,
    "c" => 3
];
$valores = array_values($array);

foreach ($valores as $valor) {
    echo "Valor: " . $valor . "<br>";
}
```

### Conversão entre Vetores e Matrizes

### Explicação
Vetores podem ser convertidos em matrizes e vice-versa, dependendo da necessidade da aplicação. A conversão é útil quando você precisa manipular os dados em diferentes formas.

### Conversão de Vetor para Matriz
```php
$vetor = [1, 2, 3, 4];
$matriz = array_chunk($vetor, 2);
// Resultado: [[1, 2], [3, 4]]
```

### Exemplo
Imagine que você deseja converter um vetor em uma matriz 2x2.

### Resolução do Exemplo
```php
$vetor = [1, 2, 3, 4];
$matriz = array_chunk($vetor, 2);

foreach ($matriz as $linha) {
    foreach ($linha as $elemento) {
        echo "Elemento: " . $elemento . "<br>";
    }
}
```

### Conversão de Matriz para Vetor
```php
$matriz = [
    [1, 2],
    [3, 4]
];
$vetor = array_merge(...$matriz);
// Resultado: [1, 2, 3, 4]
```

### Exemplo
Imagine que você deseja converter uma matriz 2x2 em um vetor.

### Resolução do Exemplo
```php
$matriz = [
    [1, 2],
    [3, 4]
];
$vetor = array_merge(...$matriz);

foreach ($vetor as $elemento) {
    echo "Elemento: " . $elemento . "<br>";
}
```

### Utilidade das Funções
- array_merge(): Combina múltiplos arrays em um único array.
- array_keys(): Extrai todas as chaves de um array associativo.
- array_values(): Extrai todos os valores de um array.
- Conversão: Permite a flexibilidade de manipular dados em diferentes formas conforme necessário.
