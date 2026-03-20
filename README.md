# 📘 Documentação da Linguagem SuperC

**SuperC** é uma linguagem de script interpretada, da família C, inspirada em Python e linguagens de script de uso simples.  
Ela suporta:

- Variáveis
- Entrada e saída no console
- Estruturas de repetição (`for`)
- Condicionais (`if-else`)

O interpretador é implementado em Python e permite executar arquivos com extensão `.supc`.

🎯 **Objetivo:**  
Focada em iniciantes na programação que querem aprender lógica.

---

## 📌 1. Estrutura do Programa

Um arquivo `.supc` é composto por linhas de código.  
Comentários podem ser inseridos usando `//` no início da linha.

### Exemplo:
    // Este é um comentário
    var x = 10
    console.write("Valor de x: ", x)

---

## 📌 2. Declaração de Variáveis

Variáveis são declaradas usando a palavra-chave `var`.

### Exemplos:
    var nome = "Alice"
    var idade = 25
    var soma = 10 + 5

- Strings devem estar entre aspas (`"`)
- Números podem ser inteiros ou decimais
- Variáveis são armazenadas em memória global

---

## 📌 3. Entrada e Saída

### 🔹 3.1 Saída no Console

    console.write("Olá, ", nome)

- Suporta múltiplos argumentos separados por vírgula
- Os valores são concatenados como strings

---

### 🔹 3.2 Entrada de Dados

**Texto:**
    var resposta = console.enterdata("Digite seu nome: ")

**Número:**
    var idade = console.enterdatanum("Digite sua idade: ")

- `console.enterdatanum` aceita apenas números válidos
- Continua pedindo até o usuário digitar corretamente

---

## 📌 4. Estruturas de Controle

### 🔹 4.1 Condicional `if-else`

    if (idade >= 18) {
       console.write("Você é maior de idade.")
    } else {
       console.write("Você é menor de idade.")
    }

- Suporta operadores: `+`, `-`, `*`, `/`, `>`, `<`, `==`, etc.
- `else` é opcional
- Blocos usam `{ }`

---

### 🔹 4.2 Laço `for (N times)`

    for (5 times) {
       console.write("Executando a iteração")
    }

- Executa o bloco **N vezes**
- `N` deve ser inteiro positivo
- Usa `{ }` para blocos

---

## 📌 5. Expressões e Avaliação

    var total = preco * quantidade
    console.write("Total: ", total)

- Variáveis podem ser usadas em expressões
- O interpretador substitui automaticamente os valores

---

## 📌 6. Comentários

    // Isso é um comentário
    var x = 10 // Comentário depois do código

- Tudo após `//` é ignorado

---

## 📌 7. Exemplo Completo

    // Programa de exemplo
    var nome = console.enterdata("Digite seu nome: ")
    var idade = console.enterdatanum("Digite sua idade: ")

    if (idade >= 18) {
       console.write("Olá ", nome, ", você é maior de idade!")
    } else {
       console.write("Olá ", nome, ", você é menor de idade!")
    }

    console.write("Vamos contar até 3:")
    for (3 times) {
       console.write("Contando...")

---

## 📌 8. Execução

Para rodar um programa `.supc`:

1. Coloque o executável da linguagem junto com o arquivo `.supc`
2. Abra a pasta no terminal (CMD)
3. Execute:

    superc.exe program.supc

📌 O interpretador:
- Lê o arquivo
- Executa linha por linha
- Processa variáveis, loops e condicionais

---

## 🚀 Contribuição

Sinta-se à vontade para contribuir com melhorias, exemplos ou correções!
