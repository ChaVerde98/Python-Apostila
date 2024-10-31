# Apostila de Introdução ao Python

---

## Sumário

1. [Sintaxe Básica](#1-sintaxe-básica)
2. [Variáveis](#2-variáveis)
3. [Tipos de Dados](#3-tipos-de-dados)
4. [Condicionais](#4-condicionais)
5. [Conversão de Tipos (Typecasting)](#5-conversão-de-tipos-typecasting)
6. [Funções](#6-funções)
7. [Estruturas de Dados - Listas, Tuplas e Conjuntos](#7-estruturas-de-dados---listas-tuplas-e-conjuntos)
8. [Dicionários](#8-dicionários)
9. [Outros](#9-outros)
---

## 1. Sintaxe Básica

Python usa indentação para definir blocos de código, como em estruturas de controle e funções. A indentação é essencial, pois Python não usa `{}` como outras linguagens.

**Importante**
- Python usa IDENTAÇÃO ao invés de `{}` então o uso dela é fundamental.


### Exemplo de Condicional Básica

```python
if 5 > 2:
    print("Cinco é maior que dois!")
```

**Explicação**:
- `if` é a palavra-chave para iniciar uma condição.
- `5 > 2` é uma condição verdadeira, então o código indentado abaixo do `if` será executado, imprimindo a mensagem `"Cinco é maior que dois!"`.

**Importante**
- Python não usa `{}` e os `()` são usados apenas em funções, então o `if` usa `:` para abrir o bloco de código. E não usa `()` para definir a condição.

---

## 2. Variáveis

Variáveis são usadas para armazenar valores que podem ser usados e modificados ao longo do código. Em Python, você não precisa declarar o tipo da variável, apenas atribuir um valor.

### Exemplo de Declaração de Variáveis

```python
nome = "Lucas"    # variável do tipo string
idade = 25        # variável do tipo inteiro
altura = 1.75     # variável do tipo float
```

**Explicação**:
- `nome` é uma variável que armazena o valor `"Lucas"`, uma string.
- `idade` armazena o valor `25`, um inteiro.
- `altura` armazena o valor `1.75`, um número decimal.

---

## 3. Tipos de Dados

Python possui tipos de dados básicos que são frequentemente utilizados:

- **Inteiros** (`int`): números inteiros, como `1`, `42`, `-7`.
- **Float** (`float`): números decimais, como `3.14`, `0.5`.
- **String** (`str`): sequência de caracteres, como `"Olá"` ou `"Python"`.
- **Booleano** (`bool`): valores lógicos, `True` ou `False`.

### Exemplo de Declaração de Diferentes Tipos

```python
num = 10          # int
preco = 9.99      # float
nome = "Ana"      # str
ativo = True      # bool
```

**Explicação**:
Cada variável acima possui um tipo de dado específico. Python identifica automaticamente o tipo com base no valor atribuído.

---

## 4. Condicionais

Estruturas condicionais permitem que o código execute instruções diferentes com base em certas condições. Em Python, usamos `if`, `elif`, e `else`.

### Exemplo de Estrutura Condicional

```python
idade = 18
if idade >= 18:
    print("Você é maior de idade.")
else:
    print("Você é menor de idade.")
```

**Explicação**:
- `if` verifica se `idade` é maior ou igual a 18.
- Se a condição é verdadeira, `print("Você é maior de idade.")` é executado.
- Caso contrário, o código no bloco `else` é executado.

---

## 5. Conversão de Tipos (Typecasting)

A conversão de tipos permite transformar dados de um tipo para outro, como transformar uma string em um número inteiro.

### Exemplo de Conversão de Tipos

```python
num_str = "10"
num_int = int(num_str)  # Converte para int
print(num_int + 5)      # Resultado: 15
```

**Explicação**:
- `num_str` é uma string que contém o valor `"10"`.
- Usamos `int(num_str)` para converter a string em um número inteiro.
- O resultado da soma é `15`, pois `num_int` agora é um número.

---


## 6. Funções

Funções são blocos de código reutilizáveis que realizam uma tarefa específica. Elas ajudam a organizar e modularizar o código. Em Python, funções são definidas com `def`.

### Exemplo de Função Simples

```python
def saudacao(nome):
    print(f"Olá, {nome}!")

saudacao("Lucas")
```

**Explicação**:
- `def saudacao(nome):` define uma função chamada `saudacao` que recebe um parâmetro `nome`.
- `print(f"Olá, {nome}!")` exibe uma mensagem personalizada.
- `saudacao("Lucas")` chama a função, passando `"Lucas"` como argumento.

---

## 7. Estruturas de Dados - Listas, Tuplas e Conjuntos

### Listas
As listas são estruturas de dados mutáveis que permitem armazenar múltiplos valores. 

#### Exemplo de Lista

```python
numeros = [1, 2, 3, 4, 5]
numeros.append(6)  # Adiciona o número 6 à lista
print(numeros)
```

**Explicação**:
- `numeros` é uma lista de inteiros.
- `append(6)` adiciona o valor `6` ao final da lista.

### Tuplas
As tuplas são estruturas de dados imutáveis. Uma vez criadas, seus valores não podem ser alterados.

#### Exemplo de Tupla

```python
coordenadas = (10, 20)
print(coordenadas[0])  # Acessa o primeiro elemento
```

**Explicação**:
- `coordenadas` é uma tupla com dois valores.
- `coordenadas[0]` acessa o primeiro elemento da tupla.

### Conjuntos
Os conjuntos são coleções de elementos únicos e não ordenados.

#### Exemplo de Conjunto

```python
frutas = {"maçã", "banana", "laranja"}
frutas.add("uva")  # Adiciona "uva" ao conjunto
print(frutas)
```

**Explicação**:
- `frutas` é um conjunto.
- `add("uva")` adiciona o item `"uva"` ao conjunto, que não permite duplicatas.

---

## 8. Dicionários

Os dicionários são coleções de pares `chave: valor`, onde cada chave é única. Eles permitem armazenar dados estruturados.

### Exemplo de Dicionário

```python
aluno = {
    "nome": "Lucas",
    "idade": 20,
    "curso": "Engenharia"
}
print(aluno["nome"])  # Acessa o valor associado à chave "nome"
```

**Explicação**:
- `aluno` é um dicionário com três pares `chave: valor`.
- `aluno["nome"]` acessa o valor `"Lucas"` associado à chave `"nome"`.

---

## 9. Outros

É interessante ter em mente conceitos anteriormente apresentados, porém não explicados.

#### - F
- `f` é uma função de formatação de strings, que permite criar strings com variáveis e/ou operações.

```python
a = 10
print("O número é: " + a) # sem formatador
print(f"O número é {a}") # com formatador
```
- Esse formatador é importante para a organização e legibilidade do código.

#### - (), [], {}
- `()` são usados para funções.
- `[]` são usados para listas ou para acessar valores com posições específicas dentro de estruturas de dados.
-  `{}` são usados para dicionários e conjuntos.


