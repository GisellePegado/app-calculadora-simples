# ⚡ Feedback Imediato ao Usuário (Real-Time Feedback)

## 💡 O que é

Feedback imediato é um princípio de design de interface em que o sistema responde à ação
do usuário **sem etapas intermediárias desnecessárias**. Quanto menor o tempo entre a
ação e a resposta visual, mais a interface parece responsiva e intuitiva.

Em calculadoras, o modelo clássico exige que o usuário pressione "=" para obter o
resultado — introduzindo um passo extra. Uma alternativa é calcular e exibir o resultado
**no próprio toque do operador**, eliminando essa etapa e tornando a interação mais direta.

Esse padrão é especialmente eficaz em apps mobile, onde reduzir o número de toques
melhora significativamente a experiência, em especial em telas pequenas.

## ⚙️ Como é usado neste projeto

A Calculadora Simples não possui botão "=". O resultado é calculado e exibido
**imediatamente ao tocar em qualquer dos 4 botões de operação** (+, −, ×, ÷).

Isso significa que, com dois números preenchidos, o usuário realiza apenas **um toque**
para obter o resultado — sem confirmar com "=". O label "RESULTADO:" é atualizado
instantaneamente após o evento de clique.

## 🔍 Exemplo do projeto

```
Fluxo tradicional (com botão "="):
  [digita 1] → [digita 5] → [toca "+"] → [toca "="] → exibe 6
  Total: 4 interações

Fluxo implementado neste app (feedback imediato):
  [digita 1] → [digita 5] → [toca "+"] → exibe 6
  Total: 3 interações

[ Quando: BotaoSoma.Clique ]
  → LabelResultado.Texto = número(TextBox1) + número(TextBox2)
  ← resultado exibido imediatamente, sem etapa adicional
```

## 📚 Recursos para aprofundamento

- [Feedback in UX Design — Nielsen Norman Group](https://www.nngroup.com/articles/response-times-3-important-limits/) — tempos de resposta e percepção do usuário
- [10 Usability Heuristics — NNg](https://www.nngroup.com/articles/ten-usability-heuristics/) — heurística #1: visibilidade do estado do sistema
- [Mobile UX Design Principles — Google](https://developer.android.com/design) — boas práticas de UX para Android
