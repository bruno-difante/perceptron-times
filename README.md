
# Perceptron_Times

Este projeto implementa um **Perceptron binário** simples em Java, treinado com dados de um arquivo CSV, com o objetivo de **classificar amostras em dois grupos distintos** (por exemplo, dois times).

## 🧠 Objetivo

Treinar um perceptron usando duas entradas numéricas (`x`, `y`) e uma saída (`-1` ou `1`), baseada em exemplos fornecidos via arquivo `CSV`.

## 📂 Estrutura do Projeto

```
Perceptron_Times/
├── amostras_saidas_problemaTimes.csv   # Arquivo com as amostras
└── src/
    └── perceptron/
        ├── Main.java
        ├── Perceptron.java
        └── Ponto.java
```

## 📄 Descrição dos Arquivos

- **Ponto.java**: representa uma amostra com dois atributos (`x`, `y`).
- **Perceptron.java**: contém a lógica de treinamento e ativação do perceptron.
- **Main.java**: ponto de entrada que:
  - Lê os dados do CSV.
  - Constrói as listas de entrada e saída.
  - Treina o perceptron.
  - Exibe os pesos finais.

## 📈 Formato do CSV

O arquivo `amostras_saidas_problemaTimes.csv` deve conter:

```
x;y;saida
```

Exemplo:

```
0.72;0.82;-1
0.91;-0.69;-1
-0.12;0.94;1
...
```

Certifique-se de que o arquivo CSV esteja na **raiz do projeto**.

## ✅ O que o programa faz

- Lê amostras com `x`, `y` e `saída esperada`.
- Treina o perceptron com os dados fornecidos.
- Ajusta os pesos sinápticos com base no erro.
- Imprime os pesos finais aprendidos após o treinamento.

## 🔚 Exemplo de saída

```
Pesos finais aprendidos pelo Perceptron:
Peso x: -0.1660
Peso y: -0.1440
Peso bias: 0.0000
```

---

Desenvolvido por Bruno Difante, para fins educacionais, com base no código original em C# fornecido pelo professor Alexandre Zamberlan.
