Repositório de Estudos: Python Essentials 1
1. Introdução
Bem-vindo ao meu repositório de estudos! Este projeto documenta minha jornada de aprendizado e conclusão do curso "Python Essentials 1" (emitido pela Cisco e OpenEDG).

O objetivo deste repositório é servir como uma base de conhecimento consolidada e um portfólio prático, demonstrando minha compreensão dos fundamentos da programação em Python. O conteúdo aqui é a base da minha preparação para desafios mais complexos na área de Ciência de Dados.

2. Conceitos Principais Abordados
Aqui estão os tópicos centrais do curso, com exemplos de código baseados em problemas que resolvi e conceitos que discutimos.

2.1. Fundamentos e Operadores
Conceitos básicos de tipos de dados, variáveis, input()/print() e os operadores matemáticos. Um foco especial foi dado aos operadores menos comuns, mas poderosos:

Módulo (%): Usado para encontrar o resto de uma divisão, essencial para lógicas como "é par ou ímpar?".

Bitwise (<<, >>, &, |): Operadores que manipulam os bits de um número, usados para otimizações e lógicas de baixo nível.

Python

# Operador de Módulo (Resto)
# Usado para checar se um número é par ou ímpar
if 5 % 2 == 1:
    print("5 é ímpar")

# Operador Bitwise Left Shift (<<)
# Dobra o valor (multiplica por 2)
# var = 1 -> 2 -> 4 -> 8 -> 16
var = 1
while var < 10:
    print("#")
    var = var << 1  # Saída: 4 hashtags
2.2. Controle de Fluxo (if, while, for)
A lógica fundamental para controlar a execução de um programa.

if, elif, else: Para tomar decisões (ex: lógica do Ano Bissexto).

while: Para loops baseados em uma condição (ex: Jogo de Adivinhação).

for: Para iterar sobre uma sequência (ex: range()).

break vs. continue:

break: Interrompe e sai do loop imediatamente.

continue: Pula a iteração atual e vai para a próxima.

Python

# Exemplo de 'break' vs. 'continue'
print("Break:")
for i in range(1, 6):
    if i == 3:
        break  # Pára o loop. Saída: 1, 2
    print(i)

print("Continue:")
for i in range(1, 6):
    if i == 3:
        continue # Pula a iteração. Saída: 1, 2, 4, 5
    print(i)
2.3. Estruturas de Dados: Listas e Tuplas
A manipulação de coleções de dados é uma das habilidades mais importantes em Python.

Criação e Indexação: Incluindo índices negativos (my_list[-1] para o último item).

Métodos de Lista:

.append(): Adiciona um item no final.

.extend(): Adiciona múltiplos itens no final.

.insert(índice, valor): Adiciona um item em uma posição específica (ex: insert(0, ...) para o início, ou o confuso insert(-1, ...) para inserir antes do último).

Remoção de Itens:

del my_list[índice]: Remove pela posição (ex: del my_list[0]).

.remove(valor): Remove o item pelo seu valor (ex: my_list.remove("John Lennon")).

Slicing (Fatiamento): A técnica mais poderosa para copiar e extrair partes de listas.

Compreensão de Listas (List Comprehension): Uma forma "Pythonica" de criar listas.

Python

# A diferença crucial entre Referência e Cópia (Slicing)

# 1. Referência (Apelido ou "Chave da Mesma Casa")
list_1 = ["A", "B", "C"]
list_2 = list_1  # list_2 é um apelido para list_1
del list_1[0]
# print(list_2) -> Saída: ['B', 'C'] (ambas mudam)

# 2. Cópia Superficial (Xerox)
list_1 = ["A", "B", "C"]
list_2 = list_1[:]  # list_2 é uma CÓPIA independente
del list_1[0]
# print(list_2) -> Saída: ['A', 'B', 'C'] (list_2 fica intacta)

# List Comprehension
# [0*0, 1*1, 2*2, 3*3, 4*4]
squares = [x * x for x in range(5)]
# squares é [0, 1, 4, 9, 16]
2.4. Funções, Escopo e Recursão
Blocos de código reutilizáveis que formam a espinha dorsal de qualquer programa.

Definição: def my_function(parametro):

Retorno: O uso de return para devolver um valor (e o que return None significa).

Escopo de Variável (Global vs. Local): O conceito mais importante. Uma variável criada dentro de uma def é local e morre com a função. A palavra-chave global é usada para forçar a modificação de uma variável externa.

Recursão: Funções que chamam a si mesmas para resolver problemas complexos (ex: fatorial ou somas).

Python

# Exemplo de Escopo Global vs. Local
a = 1  # Variável global

def fun():
    global a  # "Aviso" que vamos modificar a 'a' global
    a = 2
    print(f"Dentro da fun: {a}")

print(f"Antes de fun: {a}") # Saída: 1
fun()
print(f"Depois de fun: {a}") # Saída: 2
2.5. Tratamento de Exceções
Lidar com erros de forma elegante é o que torna um programa robusto.

Bloco try...except: Permite que o programa "tente" um código arriscado e "capture" erros específicos sem quebrar.

Tipos de Erro:

ValueError: Ex: int("banana").

TypeError: Ex: "10" / "10" (como vimos, input() retorna string!).

ZeroDivisionError: Ex: 10 / 0.

Python

# 'input()' sempre retorna STRING.
# Este código SEMPRE causará um TypeError.
try:
    value = input("Entre um valor: ")
    print(value / value)
except TypeError:
    print("Erro: Não é possível fazer divisão com texto!")
except ZeroDivisionError:
    print("Erro: Divisão por zero!")
3. Próximos Passos
A conclusão deste curso é apenas o começo. Meus próximos objetivos são:

Python Essentials 2: Aprofundar em módulos, pacotes e os fundamentos da Programação Orientada a Objetos (POO).

Bibliotecas de Data Science: Focar em Pandas e NumPy para manipulação e análise de dados.

Visualização: Aprender Matplotlib e Seaborn para criar visualizações de dados eficazes.

4. Contato
Sinta-se à vontade para se conectar comigo:

LinkedIn: www.linkedin.com/in/luasgl
