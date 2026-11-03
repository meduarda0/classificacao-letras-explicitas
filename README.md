# Classificação de Letras Explícitas em Músicas Brasileiras

Projeto desenvolvido como trabalho final do curso Ciência de Dados com Python (20h), da Universidade Federal do Piauí (UFPI).

O objetivo é desenvolver um modelo de Machine Learning capaz de classificar letras de músicas brasileiras em duas categorias: explícitas e não explícitas, utilizando técnicas de processamento de texto e aprendizado supervisionado.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Etapas do projeto

1. **Obtenção dos dados:** carregamento dos conjuntos de treinamento e teste em arquivos CSV.
2. **Limpeza e preparação:** tratamento de valores ausentes, remoção de textos vazios, conversão dos rótulos e remoção de duplicatas.
3. **Análise exploratória:** análise da distribuição das classes e da quantidade de palavras e caracteres nas letras.
4. **Pré-processamento textual:** utilização de TF-IDF para transformar os textos em representações numéricas.
5. **Modelagem:** treinamento de um classificador de Regressão Logística, utilizando divisão estratificada dos dados para treinamento e validação.
6. **Avaliação:** análise dos resultados por meio de acurácia, precisão, recall, F1-score e matriz de confusão.

## Modelo de Machine Learning

Foi desenvolvido um pipeline utilizando:

- **TF-IDF:** representação numérica dos textos, considerando unigramas e bigramas.
- **Regressão Logística:** algoritmo de classificação supervisionada para identificar padrões associados às categorias de letras explícitas e não explícitas.

O modelo utiliza os exemplos classificados presentes no conjunto de treinamento para aprender os padrões de classificação.

## Resultados

A avaliação final foi realizada em um conjunto de teste separado do treinamento.

| Métrica | Resultado |
|---|---:|
| Acurácia | 78,13% |
| Precisão | 73,58% |
| Recall | 84,78% |
| F1-score | 78,79% |

## Estrutura do projeto

```text
classificacao-letras-explicitas/
│
├── classificacao_letras_explicitas.ipynb
└── README.md
```

## Como executar

O projeto foi desenvolvido no Google Colab.

1. Clone ou baixe este repositório.
2. Abra o notebook no Google Colab ou em um ambiente Jupyter.
3. Execute as células em ordem.

As bibliotecas necessárias são:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Objetivo acadêmico

Projeto desenvolvido para aplicar conhecimentos de Ciência de Dados, análise exploratória, processamento de linguagem natural e Machine Learning, utilizando Python para resolver um problema de classificação textual.
