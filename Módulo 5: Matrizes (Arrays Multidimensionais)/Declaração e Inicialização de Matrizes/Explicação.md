
# Módulo 5: Matrizes (Arrays Multidimensionais) - Declaração e Inicialização de Matrizes

### Criação de Matrizes em PHP

### Explicação
Uma matriz em PHP é uma estrutura de dados que permite armazenar valores em múltiplas dimensões, como linhas e colunas. As matrizes são particularmente úteis para representar dados tabulares e realizar operações complexas sobre eles.

### Estrutura de Criação de Matrizes
```php
$matriz = []; // Cria uma matriz vazia
$matriz[0][0] = 1;
$matriz[0][1] = 2;
$matriz[1][0] = 3;
$matriz[1][1] = 4;
```

### Exemplo
Imagine que você deseja criar uma matriz 2x2 para armazenar valores inteiros.

### Resolução do Exemplo
```php
$matriz = []; // Criação de uma matriz vazia
$matriz[0][0] = 1;
$matriz[0][1] = 2;
$matriz[1][0] = 3;
$matriz[1][1] = 4;

for ($i = 0; $i < count($matriz); $i++) {
    for ($j = 0; $j < count($matriz[$i]); $j++) {
        echo "Elemento na posição ($i,$j): " . $matriz[$i][$j] . "<br>";
    }
}
```

### Inicialização de Matrizes com Valores

### Explicação
Você pode inicializar uma matriz com valores diretamente no momento da sua declaração, facilitando a criação de matrizes complexas de forma concisa.

### Estrutura de Inicialização de Matrizes
```php
$matriz = [
    [1, 2],
    [3, 4]
];
```

### Exemplo
Imagine que você deseja criar uma matriz 3x3 com valores predefinidos.

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

### Utilidade das Matrizes na Programação
- Armazenamento Estruturado: Matrizes são usadas para armazenar dados estruturados em múltiplas dimensões, como tabelas e grades.
- Facilitação de Operações Complexas: Matrizes permitem realizar operações matemáticas e manipulações de dados de forma eficiente.
- Acesso Rápido a Dados Relacionados: Permitem acessar dados relacionados de forma rápida e intuitiva através de índices múltiplos.

### Exemplos Comuns
- Planilhas: Representação de planilhas eletrônicas onde cada célula contém um valor específico.
- Imagens: Armazenamento de dados de pixel para processamento de imagens.
- Grades de Notas: Manter registros de notas de alunos em diferentes disciplinas.
