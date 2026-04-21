# 🧮 Operações Aritméticas (Arithmetic Operations)

## 💡 O que é

Operações aritméticas são as quatro operações matemáticas fundamentais: adição, subtração,
multiplicação e divisão. Em programação, elas são implementadas por meio de operadores
(`+`, `-`, `*`, `/`) aplicados sobre valores numéricos — inteiros ou de ponto flutuante.

Um aspecto importante em qualquer linguagem ou plataforma é a distinção entre
**divisão inteira** (que descarta o resto) e **divisão real** (que retorna o quociente
completo com casas decimais). Em calculadoras de uso geral, o comportamento esperado
é sempre a divisão real — `1 ÷ 5 = 0.2`, não `0`.

Outro ponto relevante é a **ordem de operações** (precedência): em expressões com
múltiplos operadores, multiplicação e divisão têm prioridade sobre adição e subtração.
Apps que calculam cada operação isoladamente (como este) contornam esse problema ao
limitar cada cálculo a dois operandos e um operador.

## ⚙️ Como é usado neste projeto

A Calculadora Simples implementa as 4 operações básicas, cada uma associada a um botão
dedicado. O cálculo é disparado pelo clique no botão do operador desejado, usando os
valores dos dois campos de entrada como operandos.

A divisão retorna resultado decimal quando aplicável (ex: `1 ÷ 5 = 0.2`), confirmando
que a plataforma Kodular utiliza divisão real por padrão.

## 🔍 Exemplo do projeto

```
Entradas: TextBox1 = "1"  |  TextBox2 = "5"

[ Quando: BotaoSoma.Clique ]
  → resultado = número(TextBox1) + número(TextBox2)  →  6

[ Quando: BotaoSubtracao.Clique ]
  → resultado = número(TextBox1) - número(TextBox2)  →  -4

[ Quando: BotaoMultiplicacao.Clique ]
  → resultado = número(TextBox1) × número(TextBox2)  →  5

[ Quando: BotaoDivisao.Clique ]
  → resultado = número(TextBox1) ÷ número(TextBox2)  →  0.2
```

## 📚 Recursos para aprofundamento

- [Arithmetic — Khan Academy](https://www.khanacademy.org/math/arithmetic) — fundamentos matemáticos
- [Operadores aritméticos — MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators) — implementação em código
- [Kodular Math Blocks](https://docs.kodular.io/blocks/math/) — blocos matemáticos disponíveis no Kodular
