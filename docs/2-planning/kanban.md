# 🏃 Quadro de Acompanhamento — Scrum

> Metodologia ágil aplicada ao planejamento e execução do projeto.
> As versões v1 → v8 dos APKs representam iterações sucessivas de entrega.

## 🏗️ Sprint Board

### ✅ Concluído

| Tarefa                                              | Versão | Requisito     |
| --------------------------------------------------- | ------ | ------------- |
| Protótipo de interface no Figma                     | v1     | RNF07         |
| Layout da tela com dois campos de entrada           | v1     | RF01, RF02    |
| Botões de operação (+, −, ×, ÷, C)                 | v1     | RF03–RF07     |
| Implementação da adição                             | v2     | RF03          |
| Implementação da subtração                          | v3     | RF04          |
| Implementação da multiplicação                      | v4     | RF05          |
| Implementação da divisão com suporte decimal        | v5     | RF06, RNF04   |
| Implementação do botão C (limpar)                   | v6     | RF07          |
| Validação de campos vazios                          | v7     | RF03–RF06     |
| Refinamento visual e ajustes finais                 | v8     | RNF01, RNF02  |

### 🔄 Em Revisão / Testes

| Tarefa | Requisito |
| ------ | --------- |
| (nenhuma evidência de revisão em andamento) | — |

### 🚧 Em Progresso

| Tarefa | Requisito |
| ------ | --------- |
| (nenhuma evidência de tarefa em progresso) | — |

### 📋 A Fazer

| Tarefa                                              | Prioridade | Requisito |
| --------------------------------------------------- | ---------- | --------- |
| Tratamento explícito de divisão por zero            | Alta       | RF06      |
| Histórico de operações realizadas                   | Média      | —         |
| Suporte a operações encadeadas (ex: 1+2×3)          | Baixa      | —         |
| Publicação na Google Play Store                     | Baixa      | RNF06     |

---

## 🎒 Backlog do Produto

| ID    | Item do Backlog                              | Prioridade | Requisito  |
| ----- | -------------------------------------------- | ---------- | ---------- |
| PB-01 | Operações aritméticas básicas (+, −, ×, ÷)  | Alta       | RF03–RF06  |
| PB-02 | Suporte a resultados decimais                | Alta       | RNF04      |
| PB-03 | Limpeza de campos com botão C                | Alta       | RF07       |
| PB-04 | Tratamento de divisão por zero               | Alta       | RF06       |
| PB-05 | Histórico de cálculos                        | Média      | —          |
| PB-06 | Operações encadeadas                         | Baixa      | —          |

---

## ✅ Definição de Pronto (Definition of Done - DoD)

Uma tarefa é considerada **concluída** quando:

- [ ] A funcionalidade está implementada e funcional no Kodular
- [ ] O resultado exibido é matematicamente correto para os casos testados
- [ ] O APK foi compilado e testado em dispositivo Android
- [ ] O arquivo `.apk` está disponível no repositório

---

## 🔗 Acompanhamento no GitHub

O board interativo está disponível em:

👉 [GitHub Projects →](https://github.com/GisellePegado/app-calculadora-simples/projects)
