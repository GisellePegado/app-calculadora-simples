# 🔄 Limpeza e Reset de Estado (State Reset)

## 💡 O que é

Reset de estado é a operação de devolver um sistema ao seu estado inicial, apagando todos
os dados temporários acumulados durante o uso. Em interfaces de usuário, isso é implementado
geralmente por um botão dedicado ("Limpar", "Reiniciar", "C" em calculadoras) que desfaz
todas as entradas e resultados visíveis de uma vez.

Em apps mobile, o reset de estado é especialmente importante porque o usuário frequentemente
realiza múltiplas operações em sequência sem fechar o app. Sem um mecanismo de limpeza,
o usuário precisaria apagar manualmente cada campo — o que é lento e propenso a erros
(esquecer de limpar um dos campos, por exemplo).

O botão "C" de calculadoras (de *Clear*) é uma convenção consolidada que os usuários já
conhecem — o que elimina a necessidade de explicação e reduz a curva de aprendizado.

## ⚙️ Como é usado neste projeto

O botão **"C"** da Calculadora Simples implementa o reset completo do estado do app em
um único toque: limpa o conteúdo do `TextBox1`, do `TextBox2` e do `LabelResultado`,
devolvendo a interface ao estado inicial sem precisar fechar e reabrir o app.

Esse padrão segue a convenção de calculadoras físicas e digitais amplamente conhecida.

## 🔍 Exemplo do projeto

```
Estado antes do "C":
  TextBox1 = "1"
  TextBox2 = "5"
  LabelResultado = "RESULTADO: 6"

[ Quando: BotaoLimpar.Clique ]
  → TextBox1.Texto = ""
  → TextBox2.Texto = ""
  → LabelResultado.Texto = "RESULTADO:"

Estado após o "C":
  TextBox1 = ""          (exibe placeholder "Digite o primeiro número")
  TextBox2 = ""          (exibe placeholder "Digite o segundo número")
  LabelResultado = "RESULTADO:"
```

## 📚 Recursos para aprofundamento

- [State Management in UI — UX Planet](https://uxplanet.org/state-management-in-ui-design-e2019bb5b87) — gestão de estado em interfaces
- [Clear vs Reset — UX Stack Exchange](https://ux.stackexchange.com/questions/31682/reset-vs-clear-which-button-label-is-more-appropriate) — discussão sobre nomenclatura de botões de limpeza
- [Kodular TextBox](https://docs.kodular.io/components/user-interface/textbox/) — propriedades e eventos do TextBox
