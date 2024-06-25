# Módulo 5: Matrizes (Arrays Multidimensionais) - Manipulação de Matrizes

### Acessando Elementos de uma Matriz

### Explicação
Os elementos de uma matriz podem ser acessados usando um par de índices, representando a linha e a coluna onde o elemento está localizado. Esta abordagem permite a manipulação detalhada de dados em múltiplas dimensões.

### Estrutura de Acesso
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
echo $matriz[0][1]; // Acessa o elemento na primeira linha, segunda coluna: 2
echo $matriz[2][2]; // Acessa o elemento na terceira linha, terceira coluna: 9
```

### Exemplo
Imagine que você deseja acessar os elementos na posição (1,2) e (3,3) de uma matriz.

### Resolução do Exemplo
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
echo "Elemento na posição (1,2): " . $matriz[0][1] . "<br>";
echo "Elemento na posição (3,3): " . $matriz[2][2] . "<br>";
```

### Adicionando e Removendo Elementos em Matrizes Multidimensionais

### Adicionando Elementos
Elementos podem ser adicionados em uma matriz em posições específicas, o que permite expandir e modificar a estrutura da matriz conforme necessário.

### Estrutura para Adicionar Elementos
```php
$matriz = [
    [1, 2],
    [3, 4]
];
$matriz[1][2] = 5; // Adiciona o valor 5 na segunda linha, terceira coluna
$matriz[2] = [6, 7, 8]; // Adiciona uma nova linha inteira
```

### Exemplo
Imagine que você deseja adicionar um elemento na posição (2,3) e uma nova linha na matriz.

### Resolução do Exemplo
```php
$matriz = [
    [1, 2],
    [3, 4]
];
$matriz[1][2] = 5; // Adiciona o valor 5 na segunda linha, terceira coluna
$matriz[2] = [6, 7, 8]; // Adiciona uma nova linha inteira

for ($i = 0; $i < count($matriz); $i++) {
    for ($j = 0; $j < count($matriz[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $matriz[$i][$j] . "<br>";
    }
}
```

### Removendo Elementos
Elementos podem ser removidos de uma matriz usando a função `unset()`, o que permite a manipulação dinâmica da estrutura da matriz.

### Estrutura para Remover Elementos
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
unset($matriz[0][2]); // Remove o elemento na primeira linha, terceira coluna
unset($matriz[2]); // Remove a terceira linha inteira
```

### Exemplo
Imagine que você deseja remover um elemento da posição (1,3) e uma linha inteira da matriz.

### Resolução do Exemplo
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
unset($matriz[0][2]); // Remove o elemento na primeira linha, terceira coluna
unset($matriz[2]); // Remove a terceira linha inteira

for ($i = 0; $i < count($matriz); $i++) {
    for ($j = 0; $j < count($matriz[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $matriz[$i][$j] . "<br>";
    }
}
```

### Utilidade da Manipulação de Matrizes
- Acesso Detalhado: Permite acessar e manipular dados específicos dentro de uma estrutura multidimensional.
- Flexibilidade: Adicionar e remover elementos conforme necessário para adaptar a estrutura dos dados às necessidades do programa.
- Organização Estruturada: Mantém dados organizados em múltiplas dimensões para facilitar o processamento e análise.
