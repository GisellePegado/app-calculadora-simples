# 🛠️ Requisitos Funcionais

> Derivados das Histórias de Usuário HU-01 e HU-02.

Os requisitos funcionais descrevem **o que o sistema deve fazer**.

| ID   | Nome                          | Descrição                                                                                     |
| ---- | ----------------------------- | --------------------------------------------------------------------------------------------- |
| RF01 | Entrada do primeiro número    | O app exibe um campo de texto para o usuário digitar o primeiro operando                      |
| RF02 | Entrada do segundo número     | O app exibe um campo de texto para o usuário digitar o segundo operando                       |
| RF03 | Calcular adição               | Ao tocar em "+", o app exibe a soma dos dois números em "RESULTADO:"                          |
| RF04 | Calcular subtração            | Ao tocar em "−", o app exibe a diferença dos dois números em "RESULTADO:"                     |
| RF05 | Calcular multiplicação        | Ao tocar em "×", o app exibe o produto dos dois números em "RESULTADO:"                       |
| RF06 | Calcular divisão              | Ao tocar em "÷", o app exibe o quociente dos dois números em "RESULTADO:", com suporte decimal|
| RF07 | Limpar campos e resultado     | O botão "C" apaga os dois campos de entrada e o resultado exibido                             |

---

## 🔗 Rastreabilidade: RF × Histórias de Usuário

| Requisito                  | HU-01 | HU-02 |
| -------------------------- | :---: | :---: |
| RF01 — Entrada 1º número   |  ✅   |   —   |
| RF02 — Entrada 2º número   |  ✅   |   —   |
| RF03 — Adição              |  ✅   |   —   |
| RF04 — Subtração           |  ✅   |   —   |
| RF05 — Multiplicação       |  ✅   |   —   |
| RF06 — Divisão             |  ✅   |   —   |
| RF07 — Limpar              |   —   |  ✅   |

---

## 💻 Implementação no App

| Requisito | Implementação no Kodular                                                    |
| --------- | --------------------------------------------------------------------------- |
| RF01      | Componente `TextBox` com hint "Digite o primeiro número"                    |
| RF02      | Componente `TextBox` com hint "Digite o segundo número"                     |
| RF03      | Evento clique no botão "+": converter entradas → somar → exibir no `Label` |
| RF04      | Evento clique no botão "−": converter entradas → subtrair → exibir          |
| RF05      | Evento clique no botão "×": converter entradas → multiplicar → exibir       |
| RF06      | Evento clique no botão "÷": converter entradas → dividir → exibir           |
| RF07      | Evento clique no botão "C": limpar `TextBox1`, `TextBox2` e `LabelResultado`|
