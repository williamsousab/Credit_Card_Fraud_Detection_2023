<div align="center">
<img src="https://github.com/williamsousab/Credit_Card_Fraud_Detection_2023/blob/main/images/dataset-cover%20(2).jpg?raw=true?raw=true" width="700px" />
</div>

# 💳 Credit Card Fraud Detection Dataset 2023

Detecção de fraudes em transações com cartão de crédito usando técnicas de Machine Learning. O projeto aplica diferentes modelos supervisionados e validações cruzadas para identificar transações fraudulentas com alta precisão.

---

## 📊 Dataset

- 📌 Fonte: [Kaggle - Credit Card Fraud Detection 2023](https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023)
- 💾 Total de registros: 568.630
- 🎯 Target: `Class` → 0 = legítima | 1 = fraudulenta
- ⚖️ Dados balanceados: 50% fraudes, 50% transações normais

---

## 🚀 Etapas do Projeto

### 1. Análise Exploratória

- Carregamento automático via `kagglehub`
- Verificação de:
  - Valores nulos ✅
  - Duplicatas ✅
  - Balanceamento de classes ✅

### 2. Modelagem Supervisionada

Modelos treinados com `scikit-learn`:

| Modelo              | Acurácia | Precision | Recall | F1-Score |
|---------------------|----------|-----------|--------|----------|
| Decision Tree       | 100%     | 1.00      | 1.00   | 1.00     |
| Random Forest       | **100%** | **1.00**  | **1.00** | **1.00** |
| Gradient Boosting   | 98%      | 0.97–0.99 | 0.97–0.99 | 0.98   |
| Rede Neural (MLP)   | 97%      | 0.96–0.99 | 0.96–0.99 | 0.97   |

- 🔬 Validação cruzada 5-fold
- 📊 Visualização com seaborn (matriz de confusão e distribuição por classe)

### 3. Feature Engineering

- Criadas: `V1_V2`, `log_Amount`
- Avaliadas com novos testes
- Retiradas no modelo final por não melhorarem a performance

### 4. Modelo Final

- Algoritmo: **Random Forest**
- Acurácia validada: **99.97%**
- Salvo em: `random_forest_model_final.pkl`

---

## 🧠 Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/williamsousab/credit-card-fraud-detection
cd credit-card-fraud-detection

