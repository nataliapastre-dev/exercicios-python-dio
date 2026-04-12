## 📌 Exercício 0 - Declaração de Listas

### 📂 Arquivo

`estrutura-dados/00_listas_declaracao.py`

### 🧠 Descrição

Este exercício demonstra diferentes formas de declarar listas em Python, incluindo listas com strings, listas vazias, conversão de strings em listas, uso da função `range()` e listas com múltiplos tipos de dados.

### ▶️ Código

```python id="7wz2kf"
frutas = ["laranja", "maca", "uva"]
print(frutas)

frutas = []
print(frutas)

letras = list("python")
print(letras)

numeros = list(range(10))
print(numeros)

carro = ["Ferrari", "F8", 4200000, 2020, 2900, "São Paulo", True]
print(carro)
```

### 💻 Resultado

```id="4k3snt"
['laranja', 'maca', 'uva']
[]
['p', 'y', 't', 'h', 'o', 'n']
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
['Ferrari', 'F8', 4200000, 2020, 2900, 'São Paulo', True]
```
## 📌 Exercício 1 - Acessando Elementos da Lista

### 📂 Arquivo

`estrutura-dados/01_acessando_listas.py`

### 🧠 Descrição

Este exercício demonstra como acessar elementos de uma lista utilizando índices negativos em Python. Os índices negativos permitem acessar os elementos a partir do final da lista.

### ▶️ Código

```python
frutas = ["maçã", "laranja", "uva", "pera"]

print(frutas[-1])  # pera
print(frutas[-3])  # laranja
```

### 💻 Resultado

```
pera
laranja
```
## 📌 Exercício 2 - Matrizes (Listas Aninhadas)

### 📂 Arquivo

`estrutura-dados/03_matriz.py`

### 🧠 Descrição

Este exercício demonstra o uso de listas aninhadas (matrizes) em Python, permitindo acessar elementos específicos por meio de índices. Também exemplifica o acesso a linhas e colunas utilizando índices positivos e negativos.

### ▶️ Código

```python id="ql7g9n"
matriz = [
    [1, "a", 2],
    ["b", 3, 4],
    [6, 5, "c"]
]

print(matriz[0])        # [1, "a", 2]
print(matriz[0][0])     # 1
print(matriz[0][-1])    # 2
print(matriz[-1][-1])   # "c"
```

### 💻 Resultado

```id="6q0y7s"
[1, 'a', 2]
1
2
c
```
## 📌 Exercício 4 - Método `count()`

### 📂 Arquivo

`estrutura-dados/03_count.py`

### 🧠 Descrição

Este exercício demonstra o uso do método `count()` em listas, que permite contar quantas vezes um determinado elemento aparece dentro da lista.

### ▶️ Código

```python id="p7g3kz"
cores = ["vermelho", "azul", "verde", "azul"]

print(cores.count("vermelho"))  # 1
print(cores.count("azul"))      # 2
print(cores.count("verde"))     # 1
```

### 💻 Resultado

```id="8q1xyt"
1
2
1
```
