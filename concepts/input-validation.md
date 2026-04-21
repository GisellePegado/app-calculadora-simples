# ✅ Validação de Entrada de Dados (Input Validation)

## 💡 O que é

Validação de entrada é o processo de verificar se os dados fornecidos pelo usuário estão
no formato, tipo e intervalo esperados **antes** de processá-los. Sem validação, entradas
inválidas podem causar erros de execução, resultados incorretos ou comportamento indefinido.

Em calculadoras, os casos mais comuns que exigem validação são: campos vazios (sem número
digitado), entrada não numérica (texto onde se espera número) e divisão por zero (operação
matematicamente indefinida). Cada um desses casos precisa de um tratamento explícito para
que o app se comporte de forma previsível e não trave ou exiba valores absurdos.

A validação pode ocorrer em dois momentos: **antes** do cálculo (verificando se os campos
estão preenchidos corretamente) ou **depois** (detectando resultados inválidos como `Infinity`
ou `NaN` e substituindo por uma mensagem amigável).

## ⚙️ Como é usado neste projeto

A Calculadora Simples trata a validação por meio de blocos condicionais no Kodular que
verificam se os campos estão preenchidos antes de executar o cálculo. A partir da v7,
o app passou a validar entradas vazias explicitamente.

O caso de divisão por zero é o cenário mais crítico: `1 ÷ 0` resulta em um valor
indefinido que, sem tratamento, pode exibir "Infinity" ou causar erro silencioso.

## 🔍 Exemplo do projeto

```
[ Quando: BotaoDivisao.Clique ]

  se TextBox1.Texto = "" ou TextBox2.Texto = ""
    então → LabelResultado.Texto = "Preencha os campos"

  senão se número(TextBox2) = 0
    então → LabelResultado.Texto = "Divisão por zero!"

  senão
    → LabelResultado.Texto = número(TextBox1) ÷ número(TextBox2)
```
*(Representação textual dos blocos de validação no Kodular)*

> [!NOTE]
> O tratamento de divisão por zero foi identificado como item pendente (`PB-04`)
> e pode variar entre as versões do APK.

## 📚 Recursos para aprofundamento

- [Input Validation — OWASP](https://owasp.org/www-community/controls/Input_Validation_Cheat_Sheet) — boas práticas de validação
- [Kodular Conditional Blocks](https://docs.kodular.io/blocks/control/) — blocos `if/then/else` no Kodular
- [Divisão por zero — Wikipedia](https://pt.wikipedia.org/wiki/Divis%C3%A3o_por_zero) — contexto matemático do problema
