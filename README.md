# Aula 2: Operadores em Python 🐍

## 📋 Conteúdo da Aula

Esta aula abordou os diferentes tipos de operadores disponíveis em Python, fundamentais para manipular dados e criar lógica em nossos programas.

## 📚 Operadores Estudados

### 1. Operadores Aritméticos (`operadores_aritmeticos.py`)

Os operadores básicos para realizar cálculos matemáticos:

- **Adição (`+`)**: Soma dois valores
- **Subtração (`-`)**: Subtrai o segundo valor do primeiro
- **Multiplicação (`*`)**: Multiplica dois valores
- **Divisão (`/`)**: Divide e retorna um **FLOAT**
- **Divisão Inteira (`//`)**: Divide e retorna apenas a parte inteira (**INT**)
- **Módulo (`%`)**: Retorna o resto da divisão
- **Exponenciação (`**`)**: Eleva um número a uma potência

```python
print(10 + 2)    # 12
print(10 / 2)    # 5.0 (float)
print(10 // 2)   # 5 (int)
print(10 % 3)    # 1 (resto da divisão)
print(10 ** 3)   # 1000 (10³)
```

### 2. Operadores de Associação (`operadores_associacao.py`)

Verificam se um objeto existe dentro de uma sequência:

- **`in`**: Verifica se existe
- **`not in`**: Verifica se NÃO existe

⚠️ **Importante**: São **case sensitive** (diferencia maiúsculas de minúsculas)

```python
frutas = ['limao', 'uva']
curso = 'Curso de Python'

print('limao' in frutas)     # True
print('laranja' in frutas)   # False
print('Python' in curso)    # True
print('python' in curso)    # False (case sensitive!)
```

### 3. Operadores de Atribuição (`operadores_atribuicao.py`)

Permitem atribuir e modificar valores de variáveis:

- **`=`**: Atribuição simples
- **`+=`**: Adição e atribuição
- **`-=`**: Subtração e atribuição
- **`*=`**: Multiplicação e atribuição
- **`/=`**: Divisão e atribuição
- **`//=`**: Divisão inteira e atribuição
- **`%=`**: Módulo e atribuição
- **`**=`**: Exponenciação e atribuição

```python
saldo = 500
saldo += 200  # saldo = saldo + 200
saldo *= 2    # saldo = saldo * 2
```

### 4. Operadores de Comparação (`operadores_comparacao.py`)

Comparam valores e retornam `True` ou `False`:

- **`==`**: Igualdade
- **`!=`**: Diferença
- **`>`**: Maior que
- **`>=`**: Maior ou igual
- **`<`**: Menor que
- **`<=`**: Menor ou igual

```python
saldo = 200
saque = 200

print(saldo == saque)  # True
print(saldo > saque)   # False
print(saldo >= saque)  # True
```

### 5. Operadores de Identidade (`operadores_identidade.py`)

Verificam se duas variáveis ocupam o mesmo espaço na memória:

- **`is`**: Verifica se ocupam o mesmo espaço
- **`is not`**: Verifica se NÃO ocupam o mesmo espaço

```python
curso = 'Curso de Python'
nome_curso = curso

print(curso is nome_curso)      # True
print(curso is not nome_curso)  # False
```

### 6. Operadores Lógicos (`operadores_logicos.py`)

Combinam expressões lógicas:

- **`and`**: Retorna `True` apenas se ambas as condições forem verdadeiras
- **`or`**: Retorna `True` se pelo menos uma condição for verdadeira
- **`not`**: Inverte o valor lógico

```python
saldo = 1000
saque = 250
limite = 200
conta_especial = True

# Usando and
resultado = saldo >= saque and saque <= limite

# Usando or
resultado = saldo >= saque or conta_especial

# Combinando com parênteses para clareza
resultado = (saldo >= saque and saque <= limite) or (conta_especial and saldo >= saque)
```

### 7. Precedência de Operadores (`precedencia.py`)

Python segue as regras matemáticas de precedência:

1. **Parênteses** `()`
2. **Exponenciação** `**`
3. **Multiplicação e Divisão** `*`, `/`, `//`, `%` (da esquerda para direita)
4. **Adição e Subtração** `+`, `-` (da esquerda para direita)

```python
print(10 - 5 * 2)      # 0 (não 10)
print((10 - 5) * 2)    # 10
print(10 ** 2 * 2)     # 200 (100 * 2)
print(10 / 2 * 4)      # 20.0 (5.0 * 4)
```

## 🎯 Conceitos Principais Aprendidos

- **Diferença entre `/` e `//`**: Divisão comum vs divisão inteira
- **Case Sensitivity**: Python diferencia maiúsculas de minúsculas
- **Precedência**: A ordem correta de execução das operações
- **Operadores de Identidade vs Igualdade**: `is` verifica memória, `==` verifica valor
- **Combinação de Operadores Lógicos**: Uso de parênteses para clareza

## 📁 Arquivos da Aula

- `operadores_aritmeticos.py`
- `operadores_associacao.py`
- `operadores_atribuicao.py`
- `operadores_comparacao.py`
- `operadores_identidade.py`
- `operadores_logicos.py`
- `precedencia.py`

---

*Esta aula forneceu uma base sólida sobre como manipular dados e criar lógica em Python usando os diversos tipos de operadores disponíveis na linguagem.*