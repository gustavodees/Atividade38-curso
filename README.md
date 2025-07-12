# Identificador de Números Negativos em Java

Este projeto consiste em um programa Java simples que lê uma quantidade especificada de números inteiros inseridos pelo usuário e, em seguida, exibe apenas os números negativos que foram digitados.

**Autor:** gustavodees

## Arquivos Incluídos

* `principal/Main.java`: Contém a classe principal com o método `main`, responsável por obter a entrada do usuário e identificar e exibir os números negativos.

## Como Usar

1.  **Salve o arquivo:** Salve o código fornecido em um arquivo chamado `Main.java` dentro de uma pasta chamada `principal`.
2.  **Compile o código:** Abra um terminal ou prompt de comando, navegue até o diretório raiz do seu projeto e compile o arquivo Java utilizando o compilador Java:

    ```bash
    javac principal/Main.java
    ```

3.  **Execute o programa:** Após a compilação ser concluída com sucesso, execute a classe `Main` com o comando:

    ```bash
    java principal.Main
    ```

4.  **Entrada de Dados:**
    * O programa primeiro solicitará que você digite a quantidade de números que você deseja inserir. Digite o número desejado e pressione Enter.
    * Em seguida, o programa pedirá que você digite cada um dos números, um por vez. Para cada número, digite-o e pressione Enter.

5.  **Resultado:** Após inserir todos os números, o programa exibirá a mensagem "Números negativos digitados:" seguida por cada um dos números negativos que você digitou, cada um em uma linha separada.

## Explicação do Código

### `principal/Main.java`

Este arquivo contém a classe `Main`, que é o ponto de entrada do programa.

* **Método `main`:**
    1.  Cria um objeto da classe `Scanner` para permitir a leitura de dados inseridos pelo usuário no console.
    2.  Solicita ao usuário que digite a quantidade de números que ele vai digitar e armazena esse valor na variável inteira `n`.
    3.  Cria um array de números inteiros (`int`) chamado `vect` com o tamanho especificado por `n`. Este array será utilizado para armazenar os números digitados pelo usuário.
    4.  Utiliza um loop `for` para iterar `n` vezes (para cada número que o usuário irá digitar). Em cada iteração:
        * Solicita ao usuário que digite o próximo número.
        * Lê o número inteiro inserido pelo usuário e armazena no array `vect` na posição correspondente ao índice `i`.
    5.  Imprime a mensagem "Números negativos digitados:".
    6.  Utiliza outro loop `for` para percorrer o array `vect` novamente. Em cada iteração:
        * Verifica se o número armazenado em `vect[i]` é menor que 0 (ou seja, negativo).
        * Se o número for negativo, ele é impresso no console, seguido por uma quebra de linha.
    7.  Não há necessidade de fechar o `Scanner` neste caso, pois o programa encerra logo após. No entanto, em programas mais complexos, é uma boa prática fechar o `Scanner` quando não for mais necessário para liberar recursos.
