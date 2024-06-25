# Módulo 4: Vetores (Arrays Unidimensionais) - Definição de vetores

### Explicação

Vetores, também conhecidos como arrays unidimensionais, são estruturas de dados que armazenam uma coleção de elementos de mesmo tipo. Cada elemento é acessível por um índice, o que facilita a manipulação e o armazenamento de grandes volumes de dados.

### Estrutura
```php
$nomes = ["João", "Maria", "José", "Ana"];
}
```

### Exemplo
Imagine que você deseja armazenar os nomes de quatro pessoas em uma lista para posteriormente exibir esses nomes.

### Resolução do exemplo
```php
$nomes = ["João", "Maria", "José", "Ana"];

for ($i = 0; $i < count($nomes); $i++) {
    echo "Nome: " . $nomes[$i] . "<br>";
}
```

### Utilidade dos Vetores na Programação:

- Armazenamento de Dados Relacionados: Vetores são usados para armazenar coleções de dados relacionados, como nomes, números, resultados de testes, entre outros.
- Facilidade de Acesso e Manipulação: Permitem acessar e manipular dados de forma eficiente usando índices.
- Iteração Simplificada: Vetores podem ser facilmente percorridos usando laços de repetição, tornando operações como busca e atualização de dados rápidas e simples.
- Ordenação e Pesquisa: Vetores são fundamentais para algoritmos de ordenação e pesquisa, facilitando a organização e recuperação de dados.

### Quando Usar Vetores:

- Coleções Homogêneas: Quando precisa armazenar uma coleção de elementos do mesmo tipo.
- Acesso por Índice: Quando é necessário acessar elementos específicos através de um índice.
- Operações de Iteração: Para realizar operações repetitivas sobre um conjunto de dados, como cálculo de médias, soma de valores, etc.

### Exemplos Comuns:

- Listas de Estudantes: Armazenar nomes ou notas de estudantes em uma turma.
- Inventários de Produtos: Manter uma lista de produtos em um inventário com seus preços e quantidades.
- Resultados de Testes: Guardar os resultados de testes de um software ou aplicação para análise posterior.
