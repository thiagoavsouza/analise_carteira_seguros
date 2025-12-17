# Análise de Carteira de Seguros

## Visão Geral
Este projeto apresenta uma análise de dados aplicada a uma carteira de seguros, com foco na avaliação do desempenho **comercial** e **técnico** ao longo do tempo. O estudo integra informações de vendas, produtos, filiais, frequência de sinistros e valores financeiros, permitindo identificar padrões, tendências e comportamentos relevantes para o negócio.

A análise foi desenvolvida seguindo um pipeline estruturado, combinando **Python, SQL e técnicas estatísticas**, com foco em clareza, reprodutibilidade e interpretação orientada à tomada de decisão.

---

## Objetivos
Os principais objetivos deste projeto são:
- Identificar qual filial apresenta tendência de aumento ou queda no custo médio;
- Avaliar quais produtos apresentam aumento ou queda na frequência de sinistros e no prêmio médio ao longo do período;
- Identificar as filiais com maior volume de vendas mensal;
- Identificar o produto mais vendido em cada mês.

---

## Conjunto de Dados
O conjunto de dados utilizado contém informações transacionais do setor de seguros, incluindo:
- Identificação de filial (região);
- Identificação de produto e categoria;
- Datas de referência dos registros;
- Indicadores de vendas (quantidade de registros);
- Valores de prêmio e indenização;
- Indicadores de sinistros, como quantidade e frequência.

Antes das análises, os dados passaram por etapas de:
- Conversão e padronização de tipos;
- Criação de variáveis temporais (Mês/Ano);
- Análise de valores nulos e validação de consistência.

---

## Metodologia
O pipeline analítico adotado seguiu as seguintes etapas:

1. **Carregamento e preparação dos dados em Python**  
   Conversão de tipos, tratamento de dados e criação de variáveis temporais.

2. **Persistência em banco de dados SQLite**  
   Criação de um banco intermediário para organização das análises e execução de consultas SQL.

3. **Construção de indicadores com SQL (CTEs)**  
   Agregações mensais por filial e produto, cálculo de custo médio, frequência de sinistros e métricas de vendas.

4. **Análise Exploratória de Dados (EDA)**  
   Avaliação visual e estatística para identificação de padrões, comportamentos e consistência das séries temporais.

5. **Análise de Tendência por Regressão Linear**  
   Aplicação de regressão linear em séries temporais adequadas, com interpretação baseada no slope e, quando aplicável, na significância estatística.

A regressão foi aplicada apenas em casos onde a série temporal apresentava consistência suficiente para inferência estatística.

---

## Principais Análises Realizadas
- Análise do volume de vendas por filial e por produto;
- Ranking mensal das filiais com maior volume de vendas;
- Identificação do produto mais vendido em cada mês;
- Avaliação da tendência do custo médio por filial;
- Avaliação da tendência da frequência de sinistros e do prêmio médio por produto.

---

## Resumo dos Resultados
- Uma filial apresentou liderança consistente no volume de vendas ao longo de todos os meses analisados;
- Um produto concentrou a maior parte das vendas da carteira;
- A frequência de sinistros apresentou tendência de aumento para o produto dominante;
- O prêmio médio manteve comportamento predominantemente estável.

---

## Observações
Este projeto foi desenvolvido com foco em clareza, reprodutibilidade e alinhamento entre análise técnica e interpretação de negócio, seguindo boas práticas adotadas em ambientes analíticos do setor de seguros.

---

## Principais Bibliotecas Utilizadas

```bash
pandas
numpy
matplotlib
scikit-learn
statsmodels
sqlite3
```

## Contato

E-mail: **thiago.a.v.souza@gmail.com**\
LinkedIn: **https://www.linkedin.com/in/thiagoavsouza/**
