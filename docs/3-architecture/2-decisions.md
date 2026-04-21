# ⚖️ Decisões de Arquitetura (ADRs)

## 🏛️ ADR-001 — Uso do Kodular como plataforma de desenvolvimento

**📅 Data:** 2025
**🚦 Status:** ✅ Aceita

### 💡 Contexto
O projeto é de caráter acadêmico (Aulas 5 e 6 de Fundamentos de Design de Sistemas).
Era necessária uma plataforma que permitisse criar um app Android funcional com baixa
curva de aprendizado, sem exigir linguagens nativas como Kotlin ou Java.

### 🚀 Decisão
Utilizar o **Kodular Creator** para implementar toda a lógica e interface da calculadora
por meio de blocos visuais, com compilação direta para APK Android.

### 📈 Consequências

**✅ Vantagens:**
* Sem necessidade de configurar ambiente de desenvolvimento (Android Studio, JDK, etc.)
* Compilação e exportação de APK feitas diretamente na plataforma online
* Desenvolvimento rápido adequado ao prazo acadêmico

**⚠️ Desvantagens/Riscos:**
* Projeto fica vinculado à plataforma — sem código-fonte exportável em linguagem padrão
* Limitações para funcionalidades avançadas (operações encadeadas, histórico persistente)

---

## 🏛️ ADR-002 — Cálculo imediato no clique do operador (sem botão "=")

**📅 Data:** 2025
**🚦 Status:** ✅ Aceita

### 💡 Contexto
Ao projetar o fluxo de interação da calculadora, surgiu a decisão sobre quando o cálculo
deveria ser disparado: no clique de um botão "=" dedicado (padrão de calculadoras físicas)
ou diretamente no clique do operador.

### 🚀 Decisão
Calcular e exibir o resultado **imediatamente ao tocar no botão do operador** (+, −, ×, ÷),
eliminando a necessidade de um botão "=" separado.

### 📈 Consequências

**✅ Vantagens:**
* Fluxo mais direto: o usuário realiza menos toques para obter o resultado
* Interface mais limpa com menos elementos na tela
* Feedback imediato reforça a sensação de resposta rápida (RNF01)

**⚠️ Desvantagens/Riscos:**
* Não suporta operações encadeadas naturalmente (ex: `2 + 3 × 4`)
* Comportamento diferente de calculadoras físicas tradicionais — pode surpreender o usuário

---

## 🏛️ ADR-003 — Distribuição via APK versionado no repositório

**📅 Data:** 2025
**🚦 Status:** ✅ Aceita

### 💡 Contexto
Cada iteração de desenvolvimento gerou uma nova versão funcional do app. Era necessário
um meio de distribuir e rastrear essas versões sem publicação em loja oficial.

### 🚀 Decisão
Commitar cada APK gerado no repositório GitHub com sufixo de versão (`_v2`, `_v3`...) —
totalizando 8 versões rastreadas (v1 → v8).

### 📈 Consequências

**✅ Vantagens:**
* Histórico completo de versões acessível diretamente no repositório
* Instalação imediata em qualquer Android com "fontes desconhecidas" habilitado
* Cada APK representa uma iteração de desenvolvimento documentada

**⚠️ Desvantagens/Riscos:**
* Repositório acumula tamanho a cada APK adicionado (8 arquivos binários)
* Usuário precisa habilitar instalação de fontes desconhecidas no dispositivo
