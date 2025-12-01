# 🧠 Classificação de Dígitos (MNIST) — Guia Didático

Este notebook apresenta uma revisão simples e prática dos principais conceitos de **classificação supervisionada** usando o dataset **MNIST** (imagens de dígitos escritos à mão).  
O objetivo é servir como **material introdutório** ou **apoio de aula**, para quem está retomando ou aprendendo os fundamentos de Machine Learning.

---

## 📥 1. Carregamento e Exploração Inicial

- Uso do dataset MNIST (70.000 imagens 28x28).
- Visualização das imagens para entendimento da estrutura dos dados.
- Conversão e preparação básica das features e rótulos.

---

## 🎯 2. Classificação Binária: “É o número 5?”

- Criação de um rótulo binário (5 vs. não-5).
- Treinamento de um classificador linear simples (SGD).
- Discussão sobre desbalanceamento de classes.

### 📌 Ponto Didático Importante  
A acurácia pode ser **enganosa** quando as classes são desbalanceadas.  
O notebook demonstra isso treinando um classificador que **sempre diz “não é 5”**, ainda assim obtendo uma acurácia alta.

---

## 📐 3. Métricas de Avaliação

Revisão das métricas fundamentais de classificação:

- **Precisão (Precision)**
- **Recall (Sensibilidade)**
- **Acurácia**
- **F1 Score**
- **Matriz de Confusão**

Inclui a interpretação conceitual de cada métrica e seu papel na avaliação de modelos.

---

## 🧩 4. Matriz de Confusão

- Geração da matriz de confusão do classificador binário.
- Análise dos erros mais frequentes.
- Discussão sobre falsos positivos e falsos negativos.

---

## 🔢 5. Classificação Multiclasse (0–9)

Expansão do problema para prever qualquer dígito entre 0 e 9.

Inclui:

- Validação cruzada.
- Matriz de confusão completa.
- Relatório de classificação com métricas por classe.
- Versão normalizada da matriz para analisar padrões de confusão entre dígitos.

---

## 🧭 6. Análise dos Erros

A matriz normalizada é usada para visualizar:

- Quais dígitos mais se confundem entre si.
- Padrões de erro comuns (ex.: 4 vs 9, 5 vs 3).
- Pontos de melhoria potenciais.

---

## 🏷️ 7. Classificação Multilabel

Introdução ao cenário onde cada imagem recebe **múltiplos rótulos**, como:

- Se o dígito é **maior ou igual a 7**.
- Se o dígito é **ímpar**.

Demonstra:

- Como montar múltiplas etiquetas simultaneamente.
- Uso de um classificador KNN nesse contexto.

---

## 🎓 8. Objetivo Educacional

Este notebook foi construído como material de revisão/ensino para:

- Relembrar conceitos básicos de classificação.
- Explicar métricas essenciais de avaliação.
- Mostrar por que **acurácia isolada não é suficiente**.
- Demonstrar classificação binária, multiclasse e multilabel de forma simples.
- Ilustrar erros e oportunidades de melhoria usando matrizes de confusão.