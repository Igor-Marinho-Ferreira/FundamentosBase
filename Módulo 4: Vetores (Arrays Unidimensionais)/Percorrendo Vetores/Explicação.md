
# Módulo 4: Vetores (Arrays Unidimensionais) - Percorrendo Vetores

### Uso do Laço for para Percorrer Vetores

### Explicação
O laço `for` é utilizado para percorrer vetores quando você precisa de controle total sobre os índices dos elementos. Ele permite acessar cada elemento do vetor através de seu índice, oferecendo flexibilidade para manipulações mais complexas.

### Estrutura do Laço for
```php
$vetor = [10, 20, 30, 40, 50];
for ($i = 0; $i < count($vetor); $i++) {
    echo $vetor[$i] . "<br>";
}
```

### Exemplo
Imagine que você deseja percorrer um vetor de números e imprimir cada número em uma linha separada.

### Resolução do Exemplo
```php
$numeros = [10, 20, 30, 40, 50];
for ($i = 0; $i < count($numeros); $i++) {
    echo "Número: " . $numeros[$i] . "<br>";
}
```

### Uso do Laço foreach

### Explicação
O laço `foreach` é especialmente útil para percorrer vetores de forma simples e direta. Ele itera sobre cada elemento do vetor sem a necessidade de um índice explícito, tornando o código mais legível e conciso.

### Estrutura do Laço foreach
```php
$vetor = [10, 20, 30, 40, 50];
foreach ($vetor as $valor) {
    echo $valor . "<br>";
}
```

### Exemplo
Imagine que você deseja percorrer um vetor de frutas e imprimir o nome de cada fruta em uma linha separada.

### Resolução do Exemplo
```php
$frutas = ["Maçã", "Banana", "Laranja", "Uva"];
foreach ($frutas as $fruta) {
    echo "Fruta: " . $fruta . "<br>";
}
```

### Utilidade dos Laços de Repetição
- Laço for: Ideal quando você precisa de controle sobre os índices e pode precisar manipular elementos em posições específicas.
- Laço foreach: Perfeito para percorrer vetores de forma simples e intuitiva, especialmente quando você não precisa do índice.

### Quando Usar Cada Laço
- Laço for: Use quando precisar acessar ou manipular elementos com base em seus índices. É útil em situações onde o índice é necessário para a lógica do programa.
- Laço foreach: Use quando quiser percorrer todos os elementos de um vetor de maneira simples e direta, sem a necessidade de manipular índices.

