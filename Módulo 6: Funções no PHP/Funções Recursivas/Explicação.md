
# Módulo 6: Funções no PHP - Funções Recursivas
### Definição e exemplos de funções recursivas

#### Explicação
Funções recursivas são aquelas que se chamam a si mesmas para resolver um problema menor de um problema maior. A recursão é uma técnica útil para problemas que podem ser divididos em subproblemas menores e semelhantes ao problema original.

#### Estrutura de uma função recursiva
```php
function funcaoRecursiva($parametro) {
    if (condicaoDeParada) {
        return resultado;
    } else {
        return funcaoRecursiva(novoParametro);
    }
}
```

#### Exemplo de função recursiva
Um exemplo clássico de função recursiva é o cálculo do fatorial de um número.

#### Resolução do exemplo
```php
function fatorial($n) {
    if ($n <= 1) {
        return 1;
    } else {
        return $n * fatorial($n - 1);
    }
}

echo fatorial(5); // Saída: 120
```

### Cuidados ao usar recursão

#### Explicação
Embora a recursão possa simplificar a solução de alguns problemas, é importante ter cuidado ao usá-la. Sem uma condição de parada adequada, uma função recursiva pode causar um loop infinito e eventualmente resultar em um estouro de pilha (stack overflow).

#### Dicas de boas práticas
- **Condicão de Parada:** Certifique-se de que a função tenha uma condição de parada clara e que será eventualmente alcançada.
- **Otimização:** Em alguns casos, funções recursivas podem ser otimizadas para melhorar o desempenho, como através da técnica de memoization.
- **Alternativas:** Considere se a recursão é a melhor abordagem para o problema, já que em alguns casos um loop iterativo pode ser mais eficiente.

### Exemplo de uso inadequado
```php
function somaInfinita($n) {
    return $n + somaInfinita($n + 1); // Sem condição de parada
}

echo somaInfinita(1); // Isso resultará em um erro de estouro de pilha
```

### Uso:
- Funções recursivas são ideais para problemas que podem ser naturalmente divididos em subproblemas menores e semelhantes.
- Exemplos incluem algoritmos de ordenação (como quicksort e mergesort), problemas de divisão e conquista, e cálculos matemáticos como fatorial e sequências de Fibonacci.

### Quando Usar:
- Utilize recursão quando um problema pode ser dividido em subproblemas menores e similares ao original.
- Certifique-se de que a recursão é a abordagem mais eficiente e clara para o problema em questão.
- Tenha cuidado com o desempenho e a profundidade da recursão para evitar problemas de estouro de pilha.
