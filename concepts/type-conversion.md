# 🔄 Conversão de Tipos (Type Conversion)

## 💡 O que é

Conversão de tipos (ou *type casting*) é o processo de transformar um valor de um tipo de
dado em outro. Em programação, isso é necessário quando uma operação exige um tipo específico
mas os dados disponíveis estão em outro formato.

O caso mais clássico em apps de formulário é a conversão de **string para número**: campos
de texto sempre retornam o que o usuário digitou como uma sequência de caracteres (string),
mesmo que o conteúdo seja `"42"`. Para somar, subtrair, multiplicar ou dividir, é preciso
primeiro converter essa string para um tipo numérico — caso contrário, `"1" + "5"` resulta
em `"15"` (concatenação de texto) em vez de `6` (soma aritmética).

Esse comportamento varia por linguagem: JavaScript faz coerção implícita (e silenciosa),
enquanto Python lança um erro explícito. Em plataformas visuais como o Kodular, a conversão
é feita por blocos dedicados — `number()` ou `parse number` — que transformam o texto em valor numérico.

## ⚙️ Como é usado neste projeto

O `TextBox` do Kodular sempre retorna o valor digitado como **texto**. Antes de qualquer
operação aritmética, os blocos do app convertem explicitamente o conteúdo de `TextBox1`
e `TextBox2` para número usando o bloco matemático apropriado da plataforma.

Sem essa conversão, a operação de adição entre dois campos de texto produziria concatenação
(`"1"` + `"5"` = `"15"`) em vez do resultado esperado (`6`).

## 🔍 Exemplo do projeto

```
Sem conversão (errado):
  TextBox1.Texto = "1"
  TextBox2.Texto = "5"
  resultado = TextBox1 + TextBox2  →  "15"  ❌ (concatenação de string)

Com conversão (correto):
  resultado = número(TextBox1.Texto) + número(TextBox2.Texto)  →  6  ✅

[ Quando: BotaoSoma.Clique ]
  → LabelResultado.Texto = número(TextBox1.Texto) + número(TextBox2.Texto)
```

> [!NOTE]
> Se o usuário digitar um valor não numérico (ex: "abc"), a conversão pode falhar.
> Por isso, a validação de entrada deve ocorrer **antes** da conversão de tipo.

## 📚 Recursos para aprofundamento

- [Type Conversion — MDN](https://developer.mozilla.org/pt-BR/docs/Glossary/Type_Conversion) — explicação do conceito com exemplos
- [parseInt e parseFloat — MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/parseInt) — funções de conversão em JavaScript
- [Kodular Math Blocks](https://docs.kodular.io/blocks/math/) — blocos de conversão numérica no Kodular
