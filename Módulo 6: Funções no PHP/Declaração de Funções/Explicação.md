# Módulo 6: Funções no PHP - Declaração de Funções

### Como declarar funções em PHP

#### Explicação
Declarar funções em PHP é um processo simples que envolve definir um bloco de código com um nome específico. Este nome pode ser chamado posteriormente para executar o bloco de código definido. As funções em PHP podem receber parâmetros e retornar valores, proporcionando uma grande flexibilidade no desenvolvimento de aplicações.

### Sintaxe básica de uma função
```php
function nomeDaFuncao($parametro1, $parametro2) {
    // Código a ser executado
    return $resultado;
}
```

#### Exemplo
Vamos criar uma função simples que retorna a mensagem "Olá, Mundo!".

#### Resolução do exemplo
```php
function saudacao() {
    return "Olá, Mundo!";
}

echo saudacao(); // Saída: Olá, Mundo!
```

### Uso:
- Declarar funções é essencial para a organização e modularização do código.
- Permite reutilizar o mesmo bloco de código em diferentes partes do programa, melhorando a manutenção e a legibilidade.

### Quando Usar:
- Sempre que um conjunto de operações precisar ser agrupado sob um nome único para ser reutilizado.
- Para dividir tarefas complexas em blocos menores e mais gerenciáveis.
- Para aumentar a clareza e a estrutura do código, facilitando a colaboração e a manutenção.

## Exemplos de Funções com Parâmetros

### Função para calcular a soma de dois números
```php
function soma($a, $b) {
    return $a + $b;
}

echo soma(10, 5); // Saída: 15
```

### Função para verificar se um número é par
```php
function isPar($numero) {
    return $numero % 2 == 0;
}

if (isPar(4)) {
    echo "4 é par";
} else {
    echo "4 não é par";
}
// Saída: 4 é par
```

### Uso:
- Funções com parâmetros permitem passar dados para o bloco de código, tornando-as mais dinâmicas e reutilizáveis.
- Podem ser usadas para realizar operações diversas, desde cálculos simples até processamento complexo de dados.

### Quando Usar:
- Quando uma operação precisar ser parametrizada para diferentes entradas.
- Para melhorar a modularidade e flexibilidade do código.
- Para evitar duplicação de código e facilitar atualizações futuras.
