# Loops em Python

## Resumo

### Função `range`
*   A função `range` gera uma sequência ordenada como uma lista, começando em 0 se um número inteiro positivo for fornecido.
*   Com dois parâmetros, a sequência começa no primeiro número e vai até, mas não incluindo, o segundo número.

### `For` loops
*   Os loops `for` executam uma tarefa repetidamente, como substituir cores em uma lista de quadrados.
*   A sintaxe do `for` loop permite iterar sobre listas ou tuplas, utilizando índices ou diretamente os elementos.

### `While` loops
*   Os `while` loops executam um bloco de código enquanto uma condição for verdadeira, como copiar elementos de uma lista até encontrar um que não satisfaça a condição.
*   A estrutura do `while` loop continua até que a condição se torne falsa, permitindo um controle mais dinâmico sobre a execução do código.

---

## A Função `range`

A função `range` em Python é usada para gerar uma sequência de números. É comumente usada em loops, particularmente loops `for`, para iterar sobre uma sequência de números. Aqui estão os pontos-chave sobre a função `range`:

### Sintaxe
```python
range(start, stop, step)
```

- **start** (optional): The starting value of the sequence (inclusive). Defaults to 0 if not provided.
- **stop**: The end value of the sequence (exclusive).
- **step** (optional): The difference between each number in the sequence. Defaults to 1 if not provided.

### Examples

1. **Basic Usage**:
   ```python
   for i in range(3):
       print(i)
   ```
   - **Output**: 
     ```
     0
     1
     2
     ```
   - This generates numbers from 0 to 2.

2. **Specifying Start and Stop**:
   ```python
   for i in range(2, 5):
       print(i)
   ```
   - **Output**:
     ```
     2
     3
     4
     ```
   - This generates numbers from 2 to 4.

3. **Specifying Step**:
   ```python
   for i in range(0, 10, 2):
       print(i)
   ```
   - **Output**:
     ```
     0
     2
     4
     6
     8
     ```
   - This generates even numbers from 0 to 8.

### Important Note
- In Python 3, `range` returns a range object, which is an immutable sequence type. It does not generate a list explicitly like in Python 2. If you need a list, you can convert it using `list(range(...))`.

Vamos usar um exemplo figurativo que se relaciona com o conceito de loops, especificamente os loops "for" e "while", que você aprendeu no conteúdo.

### Exemplo Figurativo: Organizando uma Festa

Imagine que você está organizando uma festa e precisa preparar uma lista de convidados. Vamos ver como os loops podem ser aplicados aqui:

- **Loop "for"**: 
  - Você tem uma lista de convidados: ["Ana", "Bruno", "Carlos", "Diana"].
  - Você quer enviar um convite para cada pessoa da lista.
  - Usando um loop "for", você pode fazer isso facilmente:
    ```python
    convidados = ["Ana", "Bruno", "Carlos", "Diana"]
    for convidado in convidados:
        print(f"Convite enviado para {convidado}!")
    ```
  - **Conexão**: Assim como no loop, você está iterando sobre cada convidado e realizando a mesma ação (enviar o convite) repetidamente.

- **Loop "while"**:
  - Agora, imagine que você está verificando se ainda há comida suficiente para os convidados. Você quer continuar servindo comida enquanto houver.
  - Você pode usar um loop "while" para isso:
    ```python
    comida_suficiente = True
    while comida_suficiente:
        print("Servindo comida...")
        # Aqui você teria uma condição que altera o valor de comida_suficiente
        # Por exemplo, se a comida acabar, você mudaria para False
    ```
  - **Conexão**: O loop "while" continua a servir comida enquanto a condição (comida suficiente) for verdadeira, assim como você faria na vida real.

### Relevância do Exemplo
- **Praticidade**: Este exemplo é relevante porque ilustra como os loops podem ser usados em situações cotidianas, como organizar uma festa, facilitando a execução de tarefas repetitivas.
- **Compreensão**: Ao relacionar a programação com uma atividade familiar, você pode entender melhor como os loops funcionam e como podem ser aplicados em diferentes contextos.

Vamos explorar alguns exemplos de código que ilustram o uso de loops em Python, especificamente os loops `for` e `while`, conforme discutido no conteúdo do curso.

### Exemplo 1: Usando um loop `for` com a função `range`

Este exemplo mostra como usar um loop `for` para substituir cores em uma lista de quadrados.

```python
# Lista de cores dos quadrados
squares = ["red", "yellow", "green"]

# Substituindo cada cor por "white"
for i in range(len(squares)):
    squares[i] = "white"

print(squares)  # Saída: ['white', 'white', 'white']
```

### Exemplo 2: Usando um loop `for` para iterar diretamente sobre uma lista

Aqui, iteramos diretamente sobre os elementos da lista sem usar índices.

```python
# Lista de cores dos quadrados
squares = ["red", "yellow", "green"]

# Exibindo cada cor
for square in squares:
    print(square)
```

### Exemplo 3: Usando `enumerate` para obter índices e elementos

Neste exemplo, usamos `enumerate` para obter tanto o índice quanto o valor de cada elemento.

```python
# Lista de cores dos quadrados
squares = ["red", "yellow", "green"]

# Exibindo o índice e a cor
for i, square in enumerate(squares):
    print(f"Index: {i}, Color: {square}")
```

### Exemplo 4: Usando um loop `while`

Este exemplo mostra como usar um loop `while` para copiar quadrados de uma lista até encontrar um quadrado de cor diferente.

```python
# Lista de cores dos quadrados
squares = ["orange", "orange", "purple", "orange"]
new_squares = []

# Copiando quadrados laranjas
i = 0
while i < len(squares) and squares[i] == "orange":
    new_squares.append(squares[i])
    i += 1

print(new_squares)  # Saída: ['orange', 'orange']
```

Esses exemplos demonstram como os loops podem ser usados para iterar sobre listas e realizar operações repetitivas de maneira eficiente. Se você tiver alguma dúvida ou precisar de mais exemplos, sinta-se à vontade para perguntar!