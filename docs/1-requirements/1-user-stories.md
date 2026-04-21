# 📖 Histórias de Usuário

> Disciplina: Fundamentos de Design de Sistemas — UNINTER (Aulas 5 e 6)

---

## 📑 HU-01 — Realizar uma operação aritmética entre dois números

**Como** usuário da calculadora,
**quero** digitar dois números e tocar em uma operação (+, −, ×, ÷),
**para que** eu veja o resultado calculado imediatamente na tela.

### ✅ Critérios de Aceitação

- [ ] O app exibe dois campos de entrada ("Digite o primeiro número" / "Digite o segundo número")
- [ ] O usuário pode digitar qualquer número inteiro ou decimal em cada campo
- [ ] Ao tocar em um dos 4 botões de operação, o resultado aparece abaixo de "RESULTADO:"
- [ ] O resultado de divisão com casas decimais é exibido corretamente (ex: 1 ÷ 5 = 0.2)
- [ ] Não é necessário tocar em um botão "=" para obter o resultado

---

## 📑 HU-02 — Limpar os campos e reiniciar o cálculo

**Como** usuário da calculadora,
**quero** tocar no botão "C" para apagar todos os valores,
**para que** eu possa iniciar um novo cálculo do zero sem fechar o app.

### ✅ Critérios de Aceitação

- [ ] O botão "C" limpa o conteúdo dos dois campos de entrada
- [ ] O botão "C" limpa o resultado exibido
- [ ] Após pressionar "C", os campos voltam a exibir os textos de placeholder

---

## 🌐 Contexto

A **Calculadora Simples** é um aplicativo Android desenvolvido com a plataforma Kodular,
com interface prototipada no Figma. O app implementa as quatro operações aritméticas básicas
(adição, subtração, multiplicação e divisão) com suporte a números decimais, dispensando
o clássico botão "=" ao calcular o resultado diretamente no toque do operador.
