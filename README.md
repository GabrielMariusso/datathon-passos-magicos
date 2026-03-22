# 🎓 Análise de Dados e Modelagem Preditiva - Passos Mágicos

Projeto desenvolvido como parte do **Datathon**, do curso de **Pós-Graduação em Data Analytics** da **FIAP (Faculdade de Informática e Administração Paulista)**.

## 👥 Integrantes do Grupo
- **Gabriel Mariusso Campachi**
- **José Eduardo Augusto Couto Fontes**
- **Mayara Soares Santos**

---

## 📌 Sobre o Repositório

Este repositório contém a **Análise Exploratória de Dados (EDA)**, o *storytelling* analítico e o código-fonte responsável pelo treinamento do **Modelo de Machine Learning** para a ONG **Passos Mágicos**.

O foco principal deste braço do projeto é extrair *insights* valiosos do histórico dos alunos (2022 a 2024) para responder às dores de negócio da associação e construir o "motor" preditivo que identifica o risco de defasagem acadêmica.

---

## 🎯 Objetivo da Análise

- Realizar a limpeza, tratamento e estruturação da base de dados fornecida.
- Responder a perguntas de negócio complexas envolvendo o desempenho, engajamento e perfil psicossocial dos alunos (IAN, IDA, IEG, IAA, IPS, IPP, IPV).
- Identificar padrões e a multidimensionalidade dos indicadores que elevam a nota global (INDE).
- Construir e validar um modelo de **Machine Learning** capaz de prever com antecedência se um aluno entrará em risco de queda de desempenho.

> 💡 **Integração** > O modelo gerado nestes notebooks é exportado e consumido em tempo real pela nossa [Aplicação Web Interativa](https://app-paapps-magicos-n8zdmdibp8vpkn3rcdiyrl.streamlit.app/), que serve como interface gerencial para a equipe pedagógica.

---

## 🧠 Desenvolvimento do Modelo (Machine Learning)

O processo de modelagem preditiva foi desenvolvido em **Python** e estruturado com rigor analítico:
- **Feature Engineering:** Tratamento de variáveis categóricas (como as Fases Quartzo, Ágata, etc.) e normalização dos indicadores de desempenho.
- **Algoritmo:** Utilizamos o algoritmo **Random Forest Classifier** (`RandomForestClassifier`), escolhido por sua robustez e alta performance na criação de múltiplas árvores de decisão para capturar padrões complexos nos dados educacionais.
- **Validação:** Separação rigorosa dos dados em conjuntos de treino e teste (`X_train`, `X_test`, etc.) para garantir que o modelo generalize bem para novos alunos.
- **Saída:** O modelo treinado foi salvo para ser embarcado no deploy da solução final.

---

## 📂 Estrutura de Arquivos

O repositório está organizado nos seguintes arquivos principais:

### 📊 `Datathon_EDA.ipynb`
- Notebook focado na **limpeza de dados** e **Análise Exploratória (EDA)**.
- Contém a criação de gráficos e visualizações para o *storytelling*.
- Traz as respostas baseadas em dados para as perguntas gerenciais da Fase 5 do Datathon.

### 🤖 `Datathon_Modelo_Preditivo.ipynb`
- Notebook dedicado exclusivamente ao **pipeline de Machine Learning**.
- Demonstra o passo a passo da engenharia de recursos, treinamento do modelo Random Forest, ajustes de hiperparâmetros e a avaliação das métricas de sucesso (Acurácia, Precisão, Recall, etc.).
