## Projeto de Data Science e Análise Não-Supervisionada - Sessões de Cinema 🎬
Este projeto aplica técnicas de Análise Não-Supervisionada para explorar padrões ocultos e detetar valores atípicos em sessões de cinema, num ciclo end-to-end de Ciência de Dados. O conjunto de dados contém variáveis relacionadas com o preço dos bilhetes, a capacidade das salas, os horários e a ocupação, tendo como variável-alvo Receita_Total. O foco principal do projeto foi segmentar sessões de cinema em perfis distintos através de clustering e detetar anomalias relevantes, permitindo compreender fenómenos como preços fora do normal, ocupações invulgares ou sessões premium.
________________________________________

## Destaques do Projeto
- Projeto avaliado com 18 valores, refletindo rigor e profundidade na aplicação de técnicas de ciência de dados e análise não-supervisionada.
- Conjunto de dados real com 142.524 registos e 14 variáveis sobre sessões de cinema.
- Aplicação de clustering utilizando os modelos K-Means e Aglomerativo Hierárquico, revelando clusters bem definidos (índices de silhueta > 0.7).
- Identificação de 5 perfis distintos de sessões de cinema, como Sessões Premium com Grande Procura ou Sessões Económicas com Baixa Procura.
- Deteção de aproximadamente 9% de valores atípicos verdadeiros utilizando o modelo Local Outlier Factor (LOF), explicados por fenómenos como promoções, salas VIP, sazonalidade e erros de registo.
________________________________________

## Resultados Principais
- Modelo K-Means: melhor configuração com 14 clusters, índice de silhueta = 0.773.
- Modelo Aglomerativo Hierárquico: melhor configuração com 12 clusters, critério de ligação de Ward e distância Euclidiana, índice de silhueta = 0.762.
- A variável Preço_Bilhete foi a mais determinante na separação dos clusters, seguida da variável Percentagem_Ocupacao_Sala.
- Os modelos K-Means e Aglomerativo Hierárquico revelaram clusters bem definidos, permitindo a identificação de 5 perfis distintos de sessões de cinema:
  1. Sessões Premium com Grande Procura
  2. Sessões Económicas com Baixa Procura
  3. Sessões Económicas e Procura Irregular
  4. Sessões com Preços Moderadamente Elevados e Procura Normal
  5. Sessões a Preço Normal e Ocupação Moderada
- Modelo Local Outlier Factor (LOF): melhor configuração com 25 vizinhos e distância do cosseno, pontuação média dos valores atípicos = 1.243. O modelo detetou cerca de 9.35% de valores atípicos verdadeiros, explicados por fenómenos como promoções, erros de registo, salas VIP e sazonalidade.
________________________________________

## Estrutura do Projeto
1. Perfilamento e pré-processamento dos dados: análise exploratória, valores omissos e atípicos, distribuições e correlações; tratamento dos valores omissos e dos valores atípicos, remoção de variáveis redundantes e de variáveis com baixa variância e discretização da variável-alvo.
2. Clustering: aplicação e avaliação dos modelos de K-Means e Aglomerativo Hierárquico através de índices internos (silhueta, inércia e Davies-Bouldin) e índices externos (pureza e rand).
3. Análise de valores atípicos: deteção utilizando o modelo Local Outlier Factor, análise bivariada de variáveis relevantes e estudo das pontuações de anomalia.
4. Avaliação detalhada: interpretação dos clusters e hipóteses para as anomalias.
________________________________________

## Ferramentas Utilizadas
- Jupyter Notebook
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
________________________________________

## Conteúdos do Repositório
- Jupyter Notebook - Projeto - Data Science e Análise Não-Supervisionada - Conjunto de Dados Cinema - Alexandre Vasconcelos.ipynb - Código do projeto
- Relatório PDF - Projeto - Data Science e Análise Não-Supervisionada - Conjunto de Dados Cinema - Alexandre Vasconcelos.pdf - Relatório do projeto, detalhado com a descrição e os resultados da análise
________________________________________

## Como Visualizar os Resultados
1. Clonar o repositório
2. Abrir no Jupyter Notebook o ficheiro `.ipynb`
3. Executar as células por ordem para reproduzir a análise
________________________________________

## Contactos
- Nome: Alexandre Vasconcelos
- Email: alex-0.5@hotmail.com
- LinkedIn: https://www.linkedin.com/in/alexandre-vasconcelos-396227167/
