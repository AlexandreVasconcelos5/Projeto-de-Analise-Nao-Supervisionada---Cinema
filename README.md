## Unsupervised ML Pipeline: Clustering & Anomaly Detection in Cinema Operations 🎬

<img width="1598" height="765" alt="Print Screen" src="https://github.com/user-attachments/assets/06ba312f-db86-4fdd-a128-4795dcf5d482" />

## Project Overview:
This project implements an end-to-end Data Science pipeline using Unsupervised Learning to uncover hidden patterns and detect operational anomalies in cinema session data. Utilizing a high-dimensional dataset (ticket pricing, hall capacity, occupancy, and scheduling hours), the core objective was to segment session profiles and isolate outliers representing promotional spikes, VIP sessions, or data entry errors.
________________________________________

## 💡Project Highlights:
- Final Grade: 19.3/20 – Post-Graduate Program in Data Science for Engineers (DaSh) @ IST, Técnico+.
- Executed rigorous data profiling and feature engineering on a high-dimensional dataset to ensure model stability.
- Implemented and optimized K-Means and Agglomerative Hierarchical models, achieving Silhouette Scores > 0.7.
- Defined 5 distinct audience profiles, such as High-Demand Premium Sessions and Low-Demand Economic Sessions, for dynamic pricing and resource allocation optimization.
- Deployed a Local Outlier Factor (LOF) model to isolate 9% of records as operational anomalies, identifying critical business insights from promotional spikes and VIP session patterns.
________________________________________

## Resultados Principais
- Os modelos K-Means e Aglomerativo Hierárquico revelaram clusters bem definidos, permitindo a identificação de 5 perfis distintos de sessões de cinema:
  1. Sessões Premium com Grande Procura
  2. Sessões Económicas com Baixa Procura
  3. Sessões Económicas e Procura Irregular
  4. Sessões com Preços Moderadamente Elevados e Procura Normal
  5. Sessões a Preço Normal e Ocupação Moderada
- Modelo Local Outlier Factor (LOF): melhor configuração com 25 vizinhos e distância do cosseno, pontuação média dos valores atípicos = 1.243. O modelo detetou cerca de 9.35% de valores atípicos, explicados por fenómenos como promoções, salas VIP, sazonalidade e erros de registo.
- Conclusão: os modelos K-Means e Aglomerativo Hierárquico apresentaram clusters bem definidos (índice de silhueta superior a 0.7), permitindo identificar perfis distintos de sessões de cinema, enquanto o modelo LOF detetou cerca de 9% de valores atípicos explicados por fenómenos reais.


## 📊 Core Results:
- K-Means Optimization: Best configuration with 14 clusters (Silhouette = 0.773).
- Hierarchical Clustering: Best configuration with 12 clusters, Ward linkage and Euclidean distance (Silhouette = 0.762).
- Feature Importance: Ticket_Price and Occupancy_Percentage were the most relevant variables for cluster differentiation.




- K-Means and Hierarchical Clustering models revealed well-defined clusters, enabling the identification of 5 distinct cinema session profiles:
    1.  High-Demand Premium Sessions
    2.  Low-Demand Economic Sessions
    3.  Irregular Demand Economic Sessions
    4.  Moderately High-Price / Normal Demand Sessions
    5.  Standard Price / Moderate Occupancy Sessions



   
- Anomaly Analysis (LOF):** Configured with 25 neighbors and Cosine distance (Mean Outlier Score = 1.243). Detected 9.35% anomalies tied to VIP hall pricing and specific seasonal campaigns.



________________________________________

## Estrutura do Projeto
1. Perfilamento e pré-processamento dos dados:
   - Análise exploratória, valores omissos e atípicos, distribuições e correlações.
   - Tratamento dos valores omissos (remoção mínima) e dos valores atípicos (truncamento aos limites mínimo e máximo).
   - Remoção de variáveis redundantes (correlação superior a 0.90) e de variáveis com baixa variância (inferior a 0.10).
   - Discretização da variável alvo em 3 classes: Baixa, Média e Alta.
     
2. Clustering:
   - Aplicação dos modelos K-Means e Aglomerativo Hierárquico.
   - Avaliação através de índices internos (silhueta, inércia e Davies-Bouldin) e índices externos (pureza e rand).
   - Interpretação dos clusters e caracterização de perfis de sessões de cinema.

3. Análise de valores atípicos:
   - Deteção utilizando o modelo LOF.
   - Análise bivariada dos pares de variáveis mais relevantes.
   - Estudo da distribuição das pontuações de anomalia e identificação de casos explicados por fenómenos reais.

4. Avaliação detalhada:
   - Interpretação dos clusters encontrados.
   - Hipóteses explicativas para as anomalias.
________________________________________

## 🛠️ Tech Stack:
- Language: Python
- Environment: Jupyter Notebook, Visual Studio Code
- Libraries: Pandas, NumPy, Scikit-learn, SciPy, Matplotlib, Seaborn
________________________________________

## 📂 Repository Structure:
- `Analise_Nao_Supervisionada_Cinema.ipynb`: Full source code and implementation.
- `Analise_Nao_Supervisionada_Cinema.pdf`: Detailed technical PDF report.
________________________________________

## 📦 Quick Start:
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Open the `.ipynb` file in Jupyter Notebook.
4. Execute cells sequentially to reproduce the analysis and visualizations.
________________________________________

## 📩 Contacts:
- Alexandre Vasconcelos
- Email: alex.vasconcelos.2057@gmail.com
- LinkedIn: [linkedin.com/in/alexandre-vasconcelos-396227167/](https://www.linkedin.com/in/alexandre-vasconcelos-396227167/)
