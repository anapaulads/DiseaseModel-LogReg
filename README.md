# 🚀 Predição de Doenças Cardiovasculares com Regressão Logística

Este projeto utiliza Machine Learning para construir um modelo preditivo de **doenças cardiovasculares**, com foco na técnica de **Regressão Logística**.  
Através da análise de dados reais de pacientes, o modelo busca identificar padrões e fatores de risco que indicam a presença ou ausência de doenças cardíacas.

---

## 📌 Objetivo

Desenvolver um modelo de classificação binária capaz de prever, com base em dados clínicos, se um paciente apresenta risco de desenvolver doenças cardiovasculares.  
O modelo pode ser usado como ferramenta auxiliar na triagem clínica ou em estudos epidemiológicos.

---

## 📁 Base de Dados

A base utilizada contém atributos clínicos e comportamentais de pacientes, como:

- **Idade**
- **Altura e Peso**
- **Glicose e Colesterol**
- **Hábito de fumar e beber álcool**
- **Pratica atividade física**
- **Presença ou ausência de doença cardiovascular (target)**

> A variável `cardio_disease` é o alvo (1 = possui doença, 0 = não possui).

---

## 📂 Estrutura do Projeto

1. **Carga de Dados**  
   - Leitura da base `CARDIO_BASE.csv` com tratamento de tipos e valores ausentes.

2. **Pré-processamento**  
   - Conversão de colunas, remoção de valores inconsistentes e balanceamento com **SMOTE**.  
   - Padronização com **StandardScaler**.

3. **Análise Exploratória (EDA)**  
   - Gráficos interativos com **Plotly** e análises com **Seaborn**.  
   - Estudo das distribuições e impacto de variáveis como colesterol, glicose, IMC, tabagismo, etc.

4. **Correlação e Multicolinearidade**  
   - Verificação com mapa de calor para entender relações entre variáveis preditoras.

5. **Divisão da Base**  
   - Separação entre treino e teste com `train_test_split`.

6. **Modelagem com Regressão Logística**  
   - Treinamento com `LogisticRegression` e avaliação nos dados de teste.

7. **Avaliação do Modelo**  
   - Métricas utilizadas: **Acurácia**, **Precisão**, **Recall**, **F1-score**.  
   - Plotagem da **Curva ROC** e cálculo do **AUC** para avaliação da performance geral.

---

## 🧪 Resultados

O modelo final demonstrou um desempenho razoável de generalização, com resultados como:

- **Acurácia**: 0.66  
- **Precisão**: 0.66  
- **Recall**: 0.66  
- **F1-score**: 0.66  
- **AUC-ROC**: 0.71

> O modelo conseguiu equilibrar bem os falsos positivos e falsos negativos, o que é crucial em contextos de saúde.

---

## 🛠 Tecnologias e Bibliotecas

- **Python**  
- **Pandas / NumPy** – manipulação de dados  
- **Seaborn / Matplotlib / Plotly** – visualizações  
- **Scikit-learn** – modelagem, avaliação e otimização  
- **Imbalanced-learn (SMOTE)** – balanceamento de dados

---

## ▶️ Como Rodar

1. Clone o repositório:
```bash
git clone https://github.com/anapaulads/DiseaseModel-LogReg.git
```
---

# 💡 Insights
Colesterol e Glicose elevados aumentam consideravelmente a chance de doença cardiovascular.

Hábitos como sedentarismo, alcoolismo e tabagismo também influenciam fortemente o risco.

Técnicas de balanceamento de dados são essenciais quando há desbalanceamento na variável alvo.

---

# 🤝 Contribuições 

Contribuições são bem-vindas!

Se você quiser sugerir melhorias, corrigir algum erro ou adicionar novas funcionalidades, siga os passos abaixo:

1. Fork este repositório
2. Crie uma branch com a sua feature:
   ```bash
   git checkout -b minha-contribuicao
   ```
3. Commit suas alterações:
    ```bash
   git commit -m 'Minha contribuição'
    ```
4. Push para a sua branch:
    ```bash
   git push origin minha-contribuicao
    ```
5. Abra um Pull Request.

---

# ✍️ Autoria
Projeto desenvolvido por Ana Paula Dias, como parte da formação em Ciência de Dados pela EBAC.
