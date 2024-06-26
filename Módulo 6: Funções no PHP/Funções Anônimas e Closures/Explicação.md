
# Módulo 6: Funções no PHP - Funções Anônimas e Closures

### Declaração de funções anônimas

#### Explicação
Funções anônimas, também conhecidas como closures, são funções que não possuem um nome especificado. Elas são úteis quando se deseja passar uma função como argumento para outra função ou quando se quer definir uma função de forma dinâmica.

#### Sintaxe básica de uma função anônima
```php
$nomeDaVariavel = function($parametro1, $parametro2) {
    // Código a ser executado
    return $resultado;
};
```

### Exemplo
Vamos criar uma função anônima que retorna a soma de dois números e armazená-la em uma variável.

### Resolução do exemplo
```php
$soma = function($a, $b) {
    return $a + $b;
};

echo $soma(10, 5); // Saída: 15
```

### Uso:
- Funções anônimas são usadas para criar blocos de código que podem ser passados como argumentos ou armazenados em variáveis.
- Elas são úteis em contextos onde a função é usada apenas uma vez ou em funções de callback.

### Quando Usar:
- Quando você precisa de uma função temporária e não deseja poluir o escopo global com nomes de funções.
- Para definir callbacks ou funções que serão passadas como argumentos para outras funções.

## Uso de closures em PHP

### Explicação
Closures em PHP são funções anônimas que podem capturar variáveis do escopo onde foram criadas. Isso permite que a função use essas variáveis mesmo quando executada fora de seu escopo original.

### Sintaxe básica de uma closure
```php
$nomeDaVariavel = function($parametro1, $parametro2) use ($var1, $var2) {
    // Código a ser executado
    return $resultado;
};
```

### Exemplo
Vamos criar uma closure que utiliza uma variável externa para calcular a soma de dois números.

### Resolução do exemplo
```php
$externa = 10;

$soma = function($a, $b) use ($externa) {
    return $a + $b + $externa;
};

echo $soma(5, 5); // Saída: 20
```

### Uso:
- Closures são usadas quando você precisa que uma função anônima acesse variáveis do escopo onde foi definida.
- Elas são úteis em programação funcional e em situações que requerem encapsulamento de dados.

### Quando Usar:
- Para criar funções dinâmicas que dependem de variáveis externas.
- Em cenários de programação assíncrona ou eventos onde a função precisa acessar variáveis do escopo externo.

### Resumo
Funções anônimas e closures são ferramentas poderosas no PHP que permitem uma maior flexibilidade e dinamismo no código. Elas são essenciais para a programação funcional e para situações onde funções temporárias ou dependentes de escopo são necessárias.
