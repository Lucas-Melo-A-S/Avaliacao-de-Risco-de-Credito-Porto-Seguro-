# 🚗 Avaliação de Risco de Crédito — Porto Seguro

## 📌 Visão geral

Este projeto tem como objetivo estimar a probabilidade de um motorista se envolver em um sinistro de seguro auto, utilizando técnicas de Machine Learning aplicadas à classificação de risco.

O estudo utiliza dados públicos da competição Safe Driver Prediction, promovida pela Porto Seguro no Kaggle. O foco não é apenas prever eventos, mas ranquear corretamente o risco, apoiando decisões como precificação e aceitação de clientes.

⸻

## 🎯 Objetivo
	•	Construir um pipeline completo de Ciência de Dados
	•	Avaliar diferentes modelos de classificação
	•	Maximizar a métrica ROC AUC, critério oficial da competição

⸻

## 🗂️ Dados
	•	Fonte: Kaggle — Safe Driver Prediction
	•	Observações: 595.212
	•	Features: 59 variáveis numéricas
	•	Target: ocorrência de sinistro
	•	Valores ausentes: codificados como -1

⸻

## 🔍 Metodologia
	•	Conversão de valores ausentes (-1 → NaN)
	•	Remoção de features com alta taxa de ausência
	•	Imputação pela média (calculada apenas no treino)
	•	Padronização das variáveis
	•	Feature selection para redução de dimensionalidade
	•	Separação entre treino, validação e teste

⸻

## 🤖 Modelos avaliados
	•	Regressão Logística (baseline)
	•	Random Forest
	•	XGBoost
	•	LightGBM
	•	CatBoost

Os modelos foram ajustados com GridSearch, utilizando ROC AUC como métrica principal.

⸻

## 📊 Resultados
	•	Random Forest apresentou forte overfitting
	•	XGBoost e LightGBM mostraram boa estabilidade
	•	CatBoost apresentou o melhor equilíbrio entre:
	•	ROC AUC
	•	Gini
	•	Generalização

⸻

## ✅ Conclusão

O CatBoost foi o modelo mais consistente para este problema, apresentando o melhor desempenho geral segundo o critério oficial da competição.

⸻

## 📁 Estrutura

├── notebook/
│   └── Teste Avaliação de Risco de Crédito (Porto Seguro).ipynb
├── README.md


⸻

## ▶️ Execução

Clone o repositório e execute o notebook principal após instalar as dependências necessárias.

⸻
