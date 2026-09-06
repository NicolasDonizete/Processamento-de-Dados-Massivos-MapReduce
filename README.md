# Processamento-de-Dados-Massivos-MapReduce
# Análise de Dados de Táxi de Nova York com MapReduce

Este repositório contém a resolução da **Atividade Avaliativa de MapReduce**, cujo objetivo é explorar o paradigma de programação **MapReduce** aplicado à análise de dados massivos, compreendendo sua estrutura, funcionamento prático e principais limitações.

A análise utiliza o conjunto de dados de viagens de táxi da cidade de Nova York (Yellow Taxi Trip Records - 2024), contendo uma amostra de 1 milhão de registros.

---

## 📌 Sumário Executivo & Questões Respondidas

O notebook `notebook.ipynb` responde explicitamente às seguintes questões usando o paradigma MapReduce em Python:

1. **Número de viagens por tipo de pagamento:** Mapeamento do código numérico de pagamento (`payment_type`) para o dicionário oficial da TLC (*Credit card, Cash, No charge, Dispute, Unknown, Voided trip*) e contagem de ocorrências.
2. **Receita total por tipo de pagamento:** Agregação do valor total arrecadado (`total_amount`) agrupado por modalidade de pagamento.
3. **Tarifa média cobrada nas viagens:** Mapeamento global para cálculo da média aritmética simples da tarifa (`fare_amount`)[cite: 1].
4. **Data e hora da viagem mais longa:** Identificação do registro de maior distância percorrida (`trip_distance`) e o respectivo carimbo de data/hora de início (`tpep_pickup_datetime`)[cite: 1].
5. **Quantidade de viagens por hora:** Extração da hora do dia (0 a 23h) a partir da data de embarque e contagem total do volume por faixa horária[cite: 1].
6. **Distância total percorrida por hora:** Acumulado das milhas percorridas pelas viagens iniciadas em cada hora do dia[cite: 1].

---

## 📂 Estrutura do Repositório

```text
.
├── notebook.ipynb        # Jupyter Notebook com a implementação completa em Python
└── README.md             # Documentação do projeto e relatório descritivo
