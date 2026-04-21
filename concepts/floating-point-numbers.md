# 🔢 Números de Ponto Flutuante (Floating-Point Numbers)

## 💡 O que é

Números de ponto flutuante são a representação computacional de números reais — ou seja,
números que podem ter parte fracionária, como `0.2`, `3.14` ou `-7.5`. O nome vem do fato
de que a vírgula decimal "flutua": a mesma quantidade de bits pode representar tanto
`0.00001` quanto `1000000.0`, dependendo do expoente.

O padrão mais utilizado é o **IEEE 754**, adotado pela maioria das linguagens e plataformas
modernas. Ele define como números decimais são armazenados em binário — o que explica
algumas peculiaridades famosas, como `0.1 + 0.2 = 0.30000000000000004` em vez de `0.3`.

Para calculadoras de uso geral, o suporte a ponto flutuante é essencial: sem ele,
`1 ÷ 5` retornaria `0` (divisão inteira) em vez de `0.2`.

## ⚙️ Como é usado neste projeto

A Calculadora Simples suporta resultados decimais, como evidenciado pela operação
`1 ÷ 5 = 0.2` observada nas telas do app. O Kodular utiliza números de ponto flutuante
por padrão em seus blocos matemáticos, então a divisão real acontece automaticamente
sem configuração adicional.

Isso significa que qualquer divisão que produza resultado fracionário será exibida
corretamente com casas decimais.

## 🔍 Exemplo do projeto

```
Operação observada nas telas do app:

  TextBox1 = "1"
  TextBox2 = "5"

  [ BotaoDivisao.Clique ]
  → resultado = número("1") ÷ número("5")
  → resultado = 1.0 ÷ 5.0
  → resultado = 0.2   ✅ (ponto flutuante)

  Se fosse divisão inteira:
  → resultado = 1 ÷ 5
  → resultado = 0      ❌ (descarta a parte decimal)
```

## 📚 Recursos para aprofundamento

- [Floating Point — Wikipedia](https://pt.wikipedia.org/wiki/V%C3%ADrgula_flutuante) — explicação detalhada do padrão IEEE 754
- [What Every Programmer Should Know About Floating-Point](https://floating-point-gui.de) — guia prático sobre armadilhas do ponto flutuante
- [Kodular Math Blocks](https://docs.kodular.io/blocks/math/) — operações numéricas disponíveis na plataforma
