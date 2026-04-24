# 🧮 Calculadora Simples — App Android

![Kodular](https://img.shields.io/badge/Kodular-Low--Code-6200EE?style=flat-square&logo=android&logoColor=white)
![Android](https://img.shields.io/badge/Android-App-3DDC84?style=flat-square&logo=android&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-brightgreen?style=flat-square)

Aplicativo Android de calculadora com as quatro operações aritméticas básicas,
desenvolvido como projeto das **Aulas 5 e 6** da disciplina **Fundamentos de Design de Sistemas**.

O app permite inserir dois números e obter o resultado imediatamente ao tocar no operador
desejado (+, −, ×, ÷), sem necessidade de confirmar com "=".

> [!NOTE]
> O projeto foi **prototipado no Figma** e **implementado no Kodular** (plataforma
> de desenvolvimento visual Android baseada em blocos), sem código nativo.

---

## 📱 Demonstração

<div align="center">

![Demonstração da Calculadora Simples](CalculadoraSimples.gif)

</div>

---

## ⬇️ Como instalar

> [!IMPORTANT]
> Ative **"Instalar apps de fontes desconhecidas"** nas configurações do seu Android
> antes de instalar o APK.

| Versão | Arquivo                                                  | O que inclui                          |
| ------ | -------------------------------------------------------- | ------------------------------------- |
| v1     | [`CalculadoraAula5e6.apk`](CalculadoraAula5e6.apk)       | Layout inicial com campos e botões    |
| v2     | [`CalculadoraAula5e6_v2.apk`](CalculadoraAula5e6_v2.apk) | + Adição                              |
| v3     | [`CalculadoraAula5e6_v3.apk`](CalculadoraAula5e6_v3.apk) | + Subtração                           |
| v4     | [`CalculadoraAula5e6_v4.apk`](CalculadoraAula5e6_v4.apk) | + Multiplicação                       |
| v5     | [`CalculadoraAula5e6_v5.apk`](CalculadoraAula5e6_v5.apk) | + Divisão com suporte decimal         |
| v6     | [`CalculadoraAula5e6_v6.apk`](CalculadoraAula5e6_v6.apk) | + Botão C (limpar)                    |
| v7     | [`CalculadoraAula5e6_v7.apk`](CalculadoraAula5e6_v7.apk) | + Validação de campos vazios          |
| v8 ✅  | [`CalculadoraAula5e6_v8.apk`](CalculadoraAula5e6_v8.apk) | Refinamentos visuais e ajustes finais |

Recomendado: instalar a versão **v8** para o app completo.

---

## 🛠️ Tecnologias utilizadas

| Ferramenta                        | Uso                                            |
| --------------------------------- | ---------------------------------------------- |
| [Kodular](https://www.kodular.io) | Desenvolvimento do app Android (visual/blocos) |
| [Figma](https://figma.com)        | Prototipagem de alta fidelidade da interface   |
| GitHub                            | Versionamento e distribuição dos APKs          |

---

## 🗂️ Documentação

A documentação completa está organizada na pasta [`docs/`](docs/):

| Categoria    | Artefatos                                                                                                                                                                                                                          |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Requisitos   | [Histórias de Usuário](docs/1-requirements/1-user-stories.md) · [Funcionais](docs/1-requirements/2-functional.md) · [Não Funcionais](docs/1-requirements/3-non-functional.md) · [Casos de Uso](docs/1-requirements/4-use-cases.md) |
| Planejamento | [Kanban / Sprint Board](docs/2-planning/kanban.md)                                                                                                                                                                                 |
| Arquitetura  | [Visão Geral](docs/3-architecture/1-overview.md) · [Decisões (ADRs)](docs/3-architecture/2-decisions.md) · [Instalação](docs/3-architecture/3-deployment.md)                                                                       |

---

## 🧠 Conceitos explorados

Este projeto documenta os seguintes conceitos na pasta [`concepts/`](concepts/):

| Conceito                                                         | Descrição resumida                                             |
| ---------------------------------------------------------------- | -------------------------------------------------------------- |
| [Operações Aritméticas](concepts/arithmetic-operations.md)       | As 4 operações e como são implementadas em blocos              |
| [Feedback Imediato ao Usuário](concepts/real-time-feedback.md)   | Resultado exibido no clique do operador, sem botão "="         |
| [Validação de Entrada de Dados](concepts/input-validation.md)    | Campos vazios e divisão por zero                               |
| [Limpeza e Reset de Estado](concepts/state-reset.md)             | Botão C devolve o app ao estado inicial                        |
| [Conversão de Tipos](concepts/type-conversion.md)                | TextBox retorna string — conversão para número antes de operar |
| [Números de Ponto Flutuante](concepts/floating-point-numbers.md) | Suporte a resultados decimais (ex: 1 ÷ 5 = 0.2)                |

> Os arquivos contêm explicações detalhadas e exemplos extraídos do projeto.

---

## 👩‍💻 Autora

_Giselle Pegado · ADS — UNINTER · 2025_
