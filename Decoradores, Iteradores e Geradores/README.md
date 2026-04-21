# 🔁 Decoradores, Iteradores e Geradores

Este projeto explora três conceitos fundamentais e poderosos do Python: **Decoradores**, **Iteradores** e **Geradores**, amplamente utilizados para escrever códigos mais organizados, reutilizáveis e eficientes.

---

## 🎯 Decoradores

Decoradores permitem **modificar ou estender o comportamento de uma função** sem alterar seu código original.

### 💡 Exemplo:

```python
def meu_decorador(funcao):
    def envelope(*args, **kwargs):
        print("Executando antes...")
        resultado = funcao(*args, **kwargs)
        print("Executando depois...")
        return resultado
    return envelope

@meu_decorador
def saudacao(nome):
    print(f"Olá {nome}!")

saudacao("João")
```

### ✅ Saída:

```
Executando antes...
Olá João!
Executando depois...
```

### 🚀 Aplicações:

* Logs
* Autenticação
* Validação de dados
* Monitoramento de execução

---

## 🔁 Iteradores

Iteradores são objetos que permitem percorrer elementos de uma coleção de forma controlada.

### 💡 Exemplo:

```python
class MeuIterador:
    def __init__(self, numeros):
        self.numeros = numeros
        self.indice = 0

    def __iter__(self):
        return self

    def __next__(self):
        if self.indice >= len(self.numeros):
            raise StopIteration

        numero = self.numeros[self.indice]
        self.indice += 1
        return numero * 2

for valor in MeuIterador([1, 2, 3]):
    print(valor)
```

### ✅ Saída:

```
2
4
6
```

### 🚀 Aplicações:

* Processamento de grandes volumes de dados
* Leitura de arquivos
* Criação de pipelines

---

## ⚡ Geradores

Geradores são uma forma mais simples de criar iteradores utilizando a palavra-chave `yield`.

### 💡 Exemplo:

```python
def meu_gerador(numeros):
    for numero in numeros:
        yield numero * 2

for valor in meu_gerador([1, 2, 3]):
    print(valor)
```

### ✅ Saída:

```
2
4
6
```

### 🚀 Vantagens:

* Menor consumo de memória
* Execução sob demanda (lazy evaluation)
* Código mais simples e legível

---

## 🔍 Comparação

| Conceito    | Complexidade | Uso de memória | Facilidade |
| ----------- | ------------ | -------------- | ---------- |
| Iteradores  | Média        | Baixo          | Médio      |
| Geradores   | Baixa        | Muito baixo    | Alto       |
| Decoradores | Média        | -              | Médio      |

---

## 🧠 Conclusão

Esses conceitos são essenciais para evoluir no Python, permitindo criar soluções mais elegantes, performáticas e reutilizáveis.

---
