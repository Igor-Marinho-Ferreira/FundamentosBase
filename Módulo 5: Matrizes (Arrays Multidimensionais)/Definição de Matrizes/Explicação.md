
# Módulo 5: Matrizes (Arrays Multidimensionais) - Definição de Matrizes

### O que são Matrizes

### Explicação
Matrizes, ou arrays multidimensionais, são estruturas de dados que permitem armazenar dados em múltiplas dimensões. Ao invés de uma única linha de elementos, como em um vetor unidimensional, uma matriz pode ser vista como uma tabela de elementos, organizada em linhas e colunas.

### Estrutura de uma Matriz
```php
$matriz = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
```

### Exemplo
Imagine que você deseja armazenar uma grade de notas de alunos, onde cada linha representa um aluno e cada coluna representa uma disciplina.

### Resolução do Exemplo
```php
$notas = [
    [7, 8, 9],
    [6, 7, 8],
    [9, 8, 7]
];

for ($i = 0; $i < count($notas); $i++) {
    for ($j = 0; $j < count($notas[$i]); $j++) {
        echo "Nota do aluno " . ($i + 1) . " na disciplina " . ($j + 1) . ": " . $notas[$i][$j] . "<br>";
    }
}
```

### Utilidade das Matrizes na Programação

### Armazenamento Estruturado
Matrizes são extremamente úteis para representar dados tabulares ou estruturados, como grades de notas, tabelas de preços, matrizes de pixels em imagens, entre outros.

### Facilitação de Operações Complexas
Ao usar matrizes, você pode facilmente realizar operações complexas como multiplicação de matrizes, transposição, e outras manipulações matemáticas.

### Acesso Rápido a Dados Relacionados
Matrizes permitem acessar rapidamente dados que estão logicamente relacionados entre si através de índices múltiplos.

### Exemplos Comuns
- Planilhas: Representação de planilhas eletrônicas onde cada célula contém um valor específico.
- Imagens: Armazenamento de dados de pixel para processamento de imagens.
- Grades de Notas:** Manter registros de notas de alunos em diferentes disciplinas.

