
# Exercícios sobre Vetores em PHP

1. **Criação de um Vetor:**
   ```php
   <?php
   $cores = ["Vermelho", "Verde", "Azul", "Amarelo"];
   foreach ($cores as $cor) {
       echo $cor . "<br>";
   }
   ?>
   ```

2. **Acessando Elementos:**
   ```php
   <?php
   $numeros = [10, 20, 30, 40, 50];
   echo "Primeiro elemento: " . $numeros[0] . "<br>";
   echo "Último elemento: " . $numeros[count($numeros) - 1] . "<br>";
   ?>
   ```

3. **Modificando Elementos:**
   ```php
   <?php
   $frutas = ["Maçã", "Banana", "Laranja"];
   $frutas[1] = "Manga";
   print_r($frutas);
   ?>
   ```

4. **Tamanho do Vetor:**
   ```php
   <?php
   $animais = ["Cachorro", "Gato", "Pássaro"];
   echo "Número de elementos no vetor: " . count($animais) . "<br>";
   ?>
   ```

5. **Adicionando Elementos:**
   ```php
   <?php
   $cidades = [];
   array_push($cidades, "São Paulo", "Rio de Janeiro", "Curitiba");
   print_r($cidades);
   ?>
   ```

6. **Iteração e Soma:**
   ```php
   <?php
   $valores = [5, 10, 15, 20, 25];
   $soma = 0;
   foreach ($valores as $valor) {
       $soma += $valor;
   }
   echo "Soma dos valores: " . $soma . "<br>";
   ?>
   ```

7. **Encontrando um Valor:**
   ```php
   <?php
   $nomes = ["Ana", "João", "Maria", "Pedro"];
   if (in_array("Maria", $nomes)) {
       echo "Maria está presente no vetor.<br>";
   } else {
       echo "Maria não está presente no vetor.<br>";
   }
   ?>
   ```

8. **Removendo Elementos:**
   ```php
   <?php
   $itens = ["Mesa", "Cadeira", "Sofá", "Cama"];
   unset($itens[array_search("Sofá", $itens)]);
   print_r($itens);
   ?>
   ```

9. **Ordenação:**
   ```php
   <?php
   $numeros = [3, 1, 4, 1, 5, 9, 2];
   sort($numeros);
   print_r($numeros);
   ?>
   ```

10. **Iteração e Média:**
    ```php
    <?php
    $notas = [7.5, 8.0, 6.5, 9.0, 7.0];
    $soma = array_sum($notas);
    $media = $soma / count($notas);
    echo "Média das notas: " . $media . "<br>";
    ?>
    ```

11. **Removendo Duplicatas:**
    ```php
    <?php
    $numeros = [1, 2, 2, 3, 4, 4, 5];
    $numeros = array_unique($numeros);
    print_r($numeros);
    ?>
    ```

12. **Vetores Associativos:**
    ```php
    <?php
    $produtos = [
        "Maçã" => 3.5,
        "Banana" => 2.0,
        "Laranja" => 4.0
    ];
    foreach ($produtos as $produto => $preco) {
        echo $produto . ": R$ " . $preco . "<br>";
    }
    ?>
    ```

13. **Invertendo um Vetor:**
    ```php
    <?php
    $letras = ['a', 'b', 'c', 'd', 'e'];
    $letras = array_reverse($letras);
    print_r($letras);
    ?>
    ```

14. **Filtro de Valores:**
    ```php
    <?php
    $idades = [12, 25, 30, 18, 21, 16];
    $idades_filtradas = array_filter($idades, function($idade) {
        return $idade >= 18;
    });
    print_r($idades_filtradas);
    ?>
    ```

15. **Busca Binária Manual:**
    ```php
    <?php
    $numeros = [10, 20, 30, 40, 50];
    $procurado = 30;
    $posicao = -1;
    foreach ($numeros as $index => $numero) {
        if ($numero == $procurado) {
            $posicao = $index;
            break;
        }
    }
    if ($posicao != -1) {
        echo "Número $procurado encontrado na posição $posicao.<br>";
    } else {
        echo "Número $procurado não encontrado.<br>";
    }
    ?>
    ```
