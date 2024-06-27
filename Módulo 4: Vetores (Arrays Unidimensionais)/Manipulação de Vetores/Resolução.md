
### Resoluções dos Exercícios

1. **Criação de um Vetor:**
   ```php
   <?php
   $livros = ["1984", "Dom Quixote", "O Senhor dos Anéis"];
   foreach ($livros as $livro) {
       echo $livro . "<br>";
   }
   ?>
   ```

2. **Acessando Elementos:**
   ```php
   <?php
   $temperaturas = [15, 20, 25, 30, 35];
   echo "O segundo elemento é: " . $temperaturas[1] . "<br>";
   echo "O quarto elemento é: " . $temperaturas[3] . "<br>";
   ?>
   ```

3. **Modificando Elementos:**
   ```php
   <?php
   $planetas = ["Terra", "Marte", "Júpiter"];
   $planetas[2] = "Saturno";
   print_r($planetas);
   ?>
   ```

4. **Tamanho do Vetor:**
   ```php
   <?php
   $filmes = ["Matrix", "Inception", "Interstellar"];
   echo "O vetor tem " . count($filmes) . " elementos.<br>";
   ?>
   ```

5. **Adicionando Elementos:**
   ```php
   <?php
   $esportes = [];
   array_push($esportes, "Futebol", "Basquete", "Vôlei");
   print_r($esportes);
   ?>
   ```

6. **Iteração e Produto:**
   ```php
   <?php
   $fatores = [2, 3, 4];
   $produto = 1;
   foreach ($fatores as $fator) {
       $produto *= $fator;
   }
   echo "O produto dos valores é: " . $produto . "<br>";
   ?>
   ```

7. **Encontrando um Valor:**
   ```php
   <?php
   $cidades = ["Paris", "Londres", "Nova York", "Tóquio"];
   if (in_array("Londres", $cidades)) {
       echo "Londres está presente no vetor.<br>";
   } else {
       echo "Londres não está presente no vetor.<br>";
   }
   ?>
   ```

8. **Removendo Elementos:**
   ```php
   <?php
   $alimentos = ["Pão", "Leite", "Queijo", "Presunto"];
   unset($alimentos[array_search("Queijo", $alimentos)]);
   print_r($alimentos);
   ?>
   ```

9. **Ordenação Decrescente:**
   ```php
   <?php
   $notas = [85, 92, 78, 88, 91];
   rsort($notas);
   print_r($notas);
   ?>
   ```

10. **Removendo Elementos com Condição:**
    ```php
    <?php
    $numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9];
    $numeros_pares = array_filter($numeros, function($numero) {
        return $numero % 2 == 0;
    });
    print_r($numeros_pares);
    ?>
    ```

11. **Calculando Mediana:**
    ```php
    <?php
    $valores = [1, 3, 3, 6, 7, 8, 9];
    sort($valores);
    $count = count($valores);
    $mediana = ($count % 2 == 0) ? ($valores[$count / 2 - 1] + $valores[$count / 2]) / 2 : $valores[floor($count / 2)];
    echo "A mediana dos valores é: " . $mediana . "<br>";
    ?>
    ```

12. **Vetor Associativo:**
    ```php
    <?php
    $estudantes = [
        "Alice" => 9.5,
        "Bob" => 8.0,
        "Carlos" => 7.0
    ];
    foreach ($estudantes as $nome => $nota) {
        echo $nome . ": " . $nota . "<br>";
    }
    ?>
    ```

13. **Filtrando Valores:**
    ```php
    <?php
    $idades = [12, 17, 19, 24, 35, 40];
    $menores_de_18 = array_filter($idades, function($idade) {
        return $idade < 18;
    });
    print_r($menores_de_18);
    ?>
    ```

14. **Concatenando Vetores:**
    ```php
    <?php
    $vetor1 = [1, 2, 3];
    $vetor2 = [4, 5, 6];
    $vetor_concatenado = array_merge($vetor1, $vetor2);
    print_r($vetor_concatenado);
    ?>
    ```

15. **Contando Frequência:**
    ```php
    <?php
    $letras = ['a', 'b', 'a', 'c', 'b', 'a'];
    $frequencia = array_count_values($letras);
    print_r($frequencia);
    ?>
    ```
