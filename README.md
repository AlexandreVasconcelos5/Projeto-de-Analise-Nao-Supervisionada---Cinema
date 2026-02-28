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
- Modelo K-Means: melhor configuração com 14 clusters, índice de silhueta = 0.773.
- Modelo Aglomerativo Hierárquico: melhor configuração com 12 clusters, critério de ligação de Ward e distância Euclidiana, índice de silhueta = 0.762.
- A variável Preço_Bilhete foi a mais relevante na separação dos clusters, seguida da variável Percentagem_Ocupacao_Sala.
- Os modelos K-Means e Aglomerativo Hierárquico revelaram clusters bem definidos, permitindo a identificação de 5 perfis distintos de sessões de cinema:
  1. Sessões Premium com Grande Procura
  2. Sessões Económicas com Baixa Procura
  3. Sessões Económicas e Procura Irregular
  4. Sessões com Preços Moderadamente Elevados e Procura Normal
  5. Sessões a Preço Normal e Ocupação Moderada
- Modelo Local Outlier Factor (LOF): melhor configuração com 25 vizinhos e distância do cosseno, pontuação média dos valores atípicos = 1.243. O modelo detetou cerca de 9.35% de valores atípicos, explicados por fenómenos como promoções, salas VIP, sazonalidade e erros de registo.
- Conclusão: os modelos K-Means e Aglomerativo Hierárquico apresentaram clusters bem definidos (índice de silhueta superior a 0.7), permitindo identificar perfis distintos de sessões de cinema, enquanto o modelo LOF detetou cerca de 9% de valores atípicos explicados por fenómenos reais.
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

## Ferramentas Utilizadas
- Jupyter Notebook
- Python
- Pandas
- NumPy
- Scikit-learn
- SciPy
- Matplotlib
- Seaborn
________________________________________

## Conteúdos do Repositório
- Analise_Nao_Supervisionada_Cinema.ipynb - Código do projeto
- Analise_Nao_Supervisionada_Cinema.pdf - Relatório do projeto, detalhado com a descrição e os resultados da análise
________________________________________

## Como Visualizar os Resultados
1. Clonar o repositório.
2. Instalar as seguintes dependências: pip install -r requirements.txt .
3. Abrir o ficheiro .ipynb no Jupyter Notebook.
4. Executar as células por ordem para reproduzir a análise.
________________________________________

- LinkedIn: https://www.linkedin.com/in/alexandre-vasconcelos-396227167/

## 📩 Contacts:
- Alexandre Vasconcelos
- Email: alex.vasconcelos.2057@gmail.com
- LinkedIn: [linkedin.com/in/alexandre-vasconcelos-396227167/](https://www.linkedin.com/in/alexandre-vasconcelos-396227167/)
