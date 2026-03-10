# 📈 Telecom X - Parte 2 - Análise de Churn de Clientes

##  Sobre o Projeto  
Este projeto tem como objetivo identificar clientes com alta probabilidade de cancelar serviços (churn) em uma empresa de telecomunicações. Ele é uma continuação do projeto anterior, Challenge Telecom X
, no qual foram realizadas análises exploratórias para compreender os fatores e padrões associados ao cancelamento de clientes da TelecomX.

Nesta etapa, aplicamos modelos de Machine Learning para analisar o comportamento dos usuários e estimar a probabilidade de churn. A partir dessas análises, foi possível identificar padrões relevantes — como tipos de contratos, métodos de pagamento e tempo de permanência — que podem influenciar a decisão de cancelamento.

Com base nesses insights, o projeto busca apoiar a criação de estratégias de retenção orientadas por dados, contribuindo para a redução do churn e para a melhoria da tomada de decisão no negócio.

---

# Relatório Detalhado de Análise de Churn de Clientes

# 📊 Previsão de Evasão de Clientes (Churn Prediction)

## 📈 Desempenho dos Modelos
> Comparação dos Modelos e Performance:
* Baseline (Dummy) – 73,92% acurácia | 0% recall → ponto de partida
* LinearSVC – 80,83% acurácia | 54% recall → melhor detecção
* Random Forest – 80,27% acurácia | 45% recall → robusto, sem escalonamento

> O LinearSVC se destacou na detecção de churn, conseguindo capturar uma parcela maior dos clientes que realmente apresentavam intenção de cancelamento.

---

## 🔍 Insights de Negócio (Feature Importance)
A análise de importância das variáveis permitiu identificar os principais fatores associados ao cancelamento de clientes (churn). Entre os principais gatilhos observados, destacam-se:

1. **Tipo de Contrato:** Clientes com contratos mensais (Month-to-Month) apresentam maior probabilidade de cancelamento, indicando menor comprometimento de longo prazo.
2. **Serviço de Internet:** Usuários de Fibra Óptica registram taxas mais elevadas de churn, o que pode refletir questões relacionadas à qualidade do serviço, suporte ou percepção de custo-benefício.
3. **Tenure (Tempo de Casa):** Clientes recém-adquiridos concentram maior risco de evasão, especialmente nos primeiros meses de contrato, caracterizando um período crítico para retenção.

---

## Conclusões e Insights
A análise revelou que o perfil do cliente propenso ao churn é multifatorial e relativamente complexo. Ainda assim, alguns padrões consistentes emergiram a partir dos dados:
*   **Duração do Contrato:** Clientes com contratos mensais (Month-to-Month) apresentam probabilidade significativamente maior de cancelar o serviço. Em contrapartida, contratos de maior duração demonstram forte associação com a retenção de clientes.
*   **Serviços de Internet e Adicionais:** O serviço de Fibra Óptica está associado a taxas mais elevadas de churn. Além disso, clientes que não utilizam serviços complementares — como Segurança Online, Backup, Proteção de Dispositivos e Suporte Técnico — apresentam maior probabilidade de cancelamento.
*   **Método de Pagamento:** O método Cheque Eletrônico aparece com maior frequência entre clientes que cancelam o serviço, sugerindo uma possível relação entre esse formato de pagamento e um perfil de cliente com maior risco de evasão.

---

## Ações Sugeridas para Reduzir Churn

1. **Promoção da Retenção de Clientes por Meio de Contratos de Longo Prazo**

* Oferecer incentivos para contratos de longo prazo, como descontos progressivos ou benefícios exclusivos para clientes que optarem por planos de 1 ou 2 anos.
* Implementar programas de fidelidade, recompensando clientes pela permanência e pelo relacionamento contínuo com a empresa.
* Destacar de forma clara os benefícios e a economia de longo prazo associados a contratos estendidos, aumentando a percepção de valor para o cliente.
* Estimular a migração de contratos mensais para planos anuais, utilizando campanhas e vantagens comerciais voltadas à retenção.

2. **Otimização da Qualidade e Percepção de Valor do Serviço de Fibra Óptica**

* Investigar os fatores específicos de churn entre clientes de Fibra Óptica, avaliando aspectos como qualidade do serviço, suporte técnico e percepção de preço.
* Desenvolver pacotes mais competitivos, incluindo benefícios adicionais ou serviços complementares gratuitos para aumentar a percepção de valor.
* Realizar auditorias na infraestrutura e na prestação do serviço de Fibra Óptica, buscando identificar e corrigir possíveis falhas que possam impactar a satisfação do cliente e contribuir para o cancelamento.

3. **Acompanhamento de Clientes Associados ao Pagamento por "Cheque Eletrônico""**

* Avaliar o processo de pagamento por "Cheque Eletrônico", identificando possíveis dificuldades operacionais ou fatores que possam estar associados a maiores taxas de cancelamento.
* Analisar a viabilidade de substituição ou redução do uso desse método, priorizando alternativas mais modernas, estáveis e automatizadas.
* Incentivar a adoção de métodos de pagamento mais seguros e automáticos, como débito automático ou cobrança recorrente, com o objetivo de reduzir o risco de churn.

---

## 🛠️ Tecnologias Utilizadas

* ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
* ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
* ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
* ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
* ![Seaborn](https://img.shields.io/badge/Seaborn-4D88FF?style=for-the-badge&logo=python&logoColor=white)
* ![Google Colab](https://img.shields.io/badge/Google%20Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
* ![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
* ![LinearSVC](https://img.shields.io/badge/LinearSVC-007ACC?style=for-the-badge&logo=python&logoColor=white)
* ![Random Forest](https://img.shields.io/badge/Random_Forest-4CAF50?style=for-the-badge&logo=python&logoColor=white)
* ![Dummy Classifier](https://img.shields.io/badge/Dummy_Classifier-9E9E9E?style=for-the-badge&logo=python&logoColor=white)
* ![OneHotEncoder](https://img.shields.io/badge/OneHotEncoder-FF9800?style=for-the-badge&logo=python&logoColor=white)
* ![StandardScaler](https://img.shields.io/badge/StandardScaler-673AB7?style=for-the-badge&logo=python&logoColor=white)

---

## 📂 Estrutura do Repositório

* `images/`: Gráficos gerados.
* `Challenge_TelecomX_Parte_2.ipynb`: Código completo e análises.
* `dados`: Base de dados [Dados Fictícios]

---

**Desenvolvido por:** Mayara Martins.<br>
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MayaraMartins95/)[![LinkedInd](https://img.shields.io/badge/LinkedIn-100000?style=for-the-badge&logo=github&logoColor=white)](https://www.linkedin.com/in/mayara-martins-rp/)
