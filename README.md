<!-- CABEÇALHO COM BADGES -->
<div align="center">

# 🐍 Python Essentials 1  
### 🧠 Repositório de Estudos e Prática — Cisco Networking Academy & OpenEDG  

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Em%20Aprendizado-success)
![License](https://img.shields.io/badge/Licença-Livre-lightgrey)
![Cisco](https://img.shields.io/badge/Cisco%20Networking%20Academy-blue?logo=cisco&logoColor=white)
![OpenEDG](https://img.shields.io/badge/OpenEDG%20Python%20Institute-FFD43B?logo=python&logoColor=blue)

</div>

---

## 1️⃣ Introdução

Bem-vindo ao meu repositório de estudos!  
Este projeto documenta minha jornada de aprendizado e conclusão do curso **"Python Essentials 1"**, oferecido pela **Cisco Networking Academy** e **OpenEDG**.

O objetivo deste repositório é servir como uma base de conhecimento consolidada e um **portfólio prático**, demonstrando minha compreensão dos fundamentos da programação em Python.  
O conteúdo aqui é a base da minha preparação para desafios mais complexos na área de **Ciência de Dados**.

---

## 2️⃣ Conceitos Principais Abordados

Aqui estão os tópicos centrais do curso, com exemplos de código baseados em problemas e conceitos abordados.

---

### 🧩 2.1 Fundamentos e Operadores

Conceitos básicos de **tipos de dados**, **variáveis**, `input()`/`print()` e operadores matemáticos.

**Operadores importantes:**
- **Módulo (%)**: Encontra o resto de uma divisão — útil para verificar se um número é par ou ímpar.
- **Bitwise (<<, >>, &, |)**: Manipulam bits — usados em otimizações e lógicas de baixo nível.

```python
# Operador de Módulo (Resto)
# Usado para checar se um número é par ou ímpar
if 5 % 2 == 1:
    print("5 é ímpar")

# Operador Bitwise Left Shift (<<)
# Dobra o valor (multiplica por 2)
var = 1
while var < 10:
    print("#")
    var = var << 1  # Saída: 4 hashtags
```

---

### 🔁 2.2 Controle de Fluxo (if, while, for)

A lógica fundamental para controlar a execução de um programa.

- `if`, `elif`, `else`: tomadas de decisão (ex: Ano Bissexto).  
- `while`: loops baseados em condição (ex: jogo de adivinhação).  
- `for`: iteração sobre sequências (ex: `range()`).  
- `break` vs `continue`: controle do fluxo interno do loop.

```python
# Exemplo de 'break' vs. 'continue'
print("Break:")
for i in range(1, 6):
    if i == 3:
        break  # Pára o loop. Saída: 1, 2
    print(i)

print("Continue:")
for i in range(1, 6):
    if i == 3:
        continue  # Pula a iteração. Saída: 1, 2, 4, 5
    print(i)
```

---

### 📋 2.3 Estruturas de Dados: Listas e Tuplas

A manipulação de coleções de dados é essencial em Python.

**Criação e Indexação:**  
Suporte a índices negativos — `my_list[-1]` acessa o último item.

**Principais métodos:**
- `.append()`: adiciona item no final.  
- `.extend()`: adiciona múltiplos itens.  
- `.insert(posição, valor)`: insere em uma posição específica.  
- `.remove(valor)` e `del lista[indice]`: removem elementos.

**Fatiamento (Slicing)** e **List Comprehension** são técnicas poderosas.

```python
# Referência vs. Cópia (Slicing)

# 1. Referência
list_1 = ["A", "B", "C"]
list_2 = list_1
del list_1[0]
print(list_2)  # Saída: ['B', 'C']

# 2. Cópia Independente
list_1 = ["A", "B", "C"]
list_2 = list_1[:]
del list_1[0]
print(list_2)  # Saída: ['A', 'B', 'C']

# List Comprehension
squares = [x * x for x in range(5)]
print(squares)  # [0, 1, 4, 9, 16]
```

---

### ⚙️ 2.4 Funções, Escopo e Recursão

Blocos de código reutilizáveis — a base da modularidade em Python.

**Conceitos-chave:**
- `def`: define funções.  
- `return`: devolve valores.  
- **Escopo Local vs Global**: variáveis criadas dentro da função são locais.  
- **Recursão**: função chamando a si mesma (ex: cálculo de fatorial).

```python
# Exemplo de Escopo Global vs. Local
a = 1  # Variável global

def fun():
    global a  # Modifica a variável global
    a = 2
    print(f"Dentro da fun: {a}")

print(f"Antes de fun: {a}")  # Saída: 1
fun()
print(f"Depois de fun: {a}")  # Saída: 2
```

---

### 🚨 2.5 Tratamento de Exceções

Lidar com erros de forma elegante torna o código mais robusto.

**Erros comuns:**
- `ValueError`: conversão inválida (`int("banana")`).  
- `TypeError`: operação com tipos incompatíveis (`"10" / "10"`).  
- `ZeroDivisionError`: divisão por zero.

```python
# Exemplo de tratamento de exceções
try:
    value = input("Entre um valor: ")
    print(value / value)
except TypeError:
    print("Erro: Não é possível fazer divisão com texto!")
except ZeroDivisionError:
    print("Erro: Divisão por zero!")
```

---

## 🚀 3️⃣ Próximos Passos

A conclusão deste curso é apenas o começo.  
Meus próximos objetivos incluem:

- **Python Essentials 2:** módulos, pacotes e POO (Programação Orientada a Objetos).  
- **Bibliotecas de Data Science:** aprofundar em `Pandas` e `NumPy`.  
- **Visualização de Dados:** aprender `Matplotlib` e `Seaborn`.

---

## 🤝 4️⃣ Contato

📫 **LinkedIn:** [www.linkedin.com/in/luasgl](https://www.linkedin.com/in/luasgl)  
💡 Sinta-se à vontade para se conectar comigo e acompanhar meus próximos projetos!

---

<div align="center">

> _“Aprender Python é aprender a pensar de forma lógica e estruturada — uma habilidade que vai muito além do código.”_  

Feito com ❤️ por **Luane Gonçalves**

</div>
