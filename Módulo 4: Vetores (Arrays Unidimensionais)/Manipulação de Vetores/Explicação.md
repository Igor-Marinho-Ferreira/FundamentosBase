
# Módulo 4: Vetores (Arrays Unidimensionais) - Manipulação de Vetores

### Acessando Elementos de um Vetor

### Explicação
Cada elemento em um vetor pode ser acessado usando um índice, que representa a posição do elemento no vetor. Os índices começam em 0.

### Estrutura de Acesso
```php
$vetor = [10, 20, 30, 40, 50];
echo $vetor[0]; // Acessa o primeiro elemento: 10
echo $vetor[3]; // Acessa o quarto elemento: 40
```

### Exemplo
Imagine que você tem um vetor de números e deseja acessar o segundo e o quinto elementos.

### Resolução do Exemplo
```php
$numeros = [10, 20, 30, 40, 50];
echo "O segundo número é: " . $numeros[1] . "<br>";
echo "O quinto número é: " . $numeros[4] . "<br>";
```

### Adicionando e Removendo Elementos

### Adicionando Elementos
Elementos podem ser adicionados ao final ou ao início de um vetor.

### Estrutura para Adicionar Elementos
```php
$vetor = [10, 20, 30];
$vetor[] = 40; // Adiciona 40 ao final do vetor
array_push($vetor, 50); // Também adiciona 50 ao final do vetor
```

### Removendo Elementos
Elementos podem ser removidos do final ou do início de um vetor.

### Estrutura para Remover Elementos
```php
$vetor = [10, 20, 30, 40, 50];
array_pop($vetor); // Remove o último elemento: 50
array_shift($vetor); // Remove o primeiro elemento: 10
```

### Exemplo
Imagine que você deseja adicionar um novo número ao início e ao final do vetor e depois remover um número do início e do final.

### Resolução do Exemplo
```php
$numeros = [20, 30, 40];
array_unshift($numeros, 10); // Adiciona 10 ao início do vetor
array_push($numeros, 50); // Adiciona 50 ao final do vetor

echo "Após adicionar: ";
print_r($numeros);

array_shift($numeros); // Remove o primeiro elemento
array_pop($numeros); // Remove o último elemento

echo "<br>Após remover: ";
print_r($numeros);
```

### Funções Úteis

### count()
A função `count()` retorna o número de elementos em um vetor.

### Exemplo
```php
$vetor = [10, 20, 30, 40, 50];
echo "O vetor tem " . count($vetor) . " elementos.";
```

### array_push()
A função `array_push()` adiciona um ou mais elementos ao final de um vetor.

### Exemplo
```php
$vetor = [10, 20, 30];
array_push($vetor, 40, 50);
print_r($vetor); // [10, 20, 30, 40, 50]
```

### array_pop()
A função `array_pop()` remove e retorna o último elemento de um vetor.

### Exemplo
```php
$vetor = [10, 20, 30];
$ultimo = array_pop($vetor);
echo "Removido: " . $ultimo; // Removido: 30
print_r($vetor); // [10, 20]
```

### array_shift()
A função `array_shift()` remove e retorna o primeiro elemento de um vetor.

### Exemplo
```php
$vetor = [10, 20, 30];
$primeiro = array_shift($vetor);
echo "Removido: " . $primeiro; // Removido: 10
print_r($vetor); // [20, 30]
```

### array_unshift()
A função `array_unshift()` adiciona um ou mais elementos ao início de um vetor.

### Exemplo
```php
$vetor = [20, 30];
array_unshift($vetor, 10);
print_r($vetor); // [10, 20, 30]
```

### Utilidade das Funções
- count():** Útil para obter o número de elementos em um vetor, especialmente em loops.
- array_push():** Simplifica a adição de múltiplos elementos ao final do vetor.
- array_pop():** Facilita a remoção do último elemento quando a ordem importa.
- array_shift():** Útil para remover o primeiro elemento quando necessário.
- array_unshift():** Simplifica a adição de elementos ao início do vetor.
