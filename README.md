# Projeto Final de Ciência de Dados Aplicada

## Visão Geral
Bem-vindo ao Projeto Final de Ciência de Dados Aplicada, onde embarcamos em uma jornada para prever o pouso bem-sucedido do primeiro estágio do Falcon 9. A SpaceX, conhecida por revolucionar as viagens espaciais, anuncia lançamentos de foguetes Falcon 9 a um custo competitivo de 62 milhões de dólares, comparado aos custos de outros fornecedores que ultrapassam 165 milhões de dólares. Essa economia significativa é atribuída principalmente à capacidade da SpaceX de reutilizar o primeiro estágio do foguete. Ao prever com precisão o sucesso do pouso do primeiro estágio, podemos estimar melhor os custos de lançamento, fornecendo insights valiosos para empresas que competem com a SpaceX em lançamentos de foguetes.

## Objetivos
O projeto está estruturado em vários módulos abrangentes, cada um desenvolvido com base no anterior, culminando em um modelo preditivo robusto. Abaixo está uma descrição detalhada das tarefas e metas alcançadas em cada módulo:

### 1. Requisição à API da SpaceX e Limpeza de Dados
- **Coleta de Dados**: Iniciamos nosso projeto fazendo uma requisição GET à API da SpaceX para coletar dados históricos de lançamentos. Esses dados incluíam vários parâmetros essenciais para nossa análise.
- **Limpeza de Dados**: Após obter os dados, realizamos limpeza e formatação para garantir consistência, removendo quaisquer anomalias ou valores ausentes, e preparando-os para análise.

### 2. Web Scraping de Registros de Lançamento do Falcon 9
- **Web Scraping com BeautifulSoup**: Extraímos registros de lançamento do Falcon 9 da Wikipedia usando BeautifulSoup, uma biblioteca Python poderosa para web scraping.
- **Análise de Dados**: A tabela HTML extraída foi analisada e convertida em um DataFrame Pandas, facilitando a manipulação e análise dos dados.

### 3. Análise Exploratória de Dados (EDA) e Rótulos de Treinamento
- **Análise Exploratória de Dados**: Conduzimos extensa EDA usando ferramentas de visualização como Matplotlib e Seaborn para descobrir padrões e correlações nos dados.
- **Rótulos de Treinamento**: Identificamos e rotulamos os dados de treinamento, cruciais para os modelos de machine learning subsequentes.

### 4. Integração com Banco de Dados
- **Carregamento de Dados no Db2**: Carregamos o conjunto de dados em um banco de dados Db2 para aproveitar o SQL para consultas e análises estruturadas.
- **Execução de Consultas SQL**: Executamos várias consultas SQL para obter insights e responder perguntas específicas relacionadas aos dados de lançamento.

### 5. Engenharia de Atributos e Visualização
- **Engenharia de Atributos**: Criamos novos atributos a partir dos dados existentes para aumentar o poder preditivo de nossos modelos.
- **Visualização com Folium**: Usamos Folium para criar mapas interativos, marcando locais de lançamento e visualizando taxas de sucesso e falha, ajudando a identificar padrões geográficos.

### 6. Análise Visual Interativa com Plotly Dash
- **Construção da Aplicação Dash**: Desenvolvemos uma aplicação interativa Plotly Dash, permitindo que usuários realizem análises visuais em tempo real dos dados de lançamento da SpaceX.
- **Componentes de Interação do Usuário**: Incorporamos listas suspensas e controles deslizantes de intervalo para permitir interação dinâmica com gráficos de pizza e dispersão, tornando a análise mais intuitiva e envolvente.

### 7. Modelos de Machine Learning e Ajuste de Hiperparâmetros
- **Padronização e Divisão de Dados**: Padronizamos o conjunto de dados e o dividimos em conjuntos de treinamento e teste para garantir uma avaliação robusta do modelo.
- **Ajuste de Hiperparâmetros**: Realizamos ajuste de hiperparâmetros usando GridSearchCV para vários modelos, incluindo SVM, Árvores de Classificação e Regressão Logística.
- **Avaliação de Modelos**: Avaliamos o desempenho de cada modelo nos dados de teste para identificar o modelo com melhor performance.

## Resultados
- **Classificador de Árvore de Decisão**: Alcançou a maior precisão de 0,9444 no conjunto de teste, tornando-se o modelo com melhor desempenho.
- **SVM e K-Vizinhos Mais Próximos**: Ambos os modelos atingiram precisão de 0,8333 no conjunto de teste.

## Conclusão
Através de análise meticulosa de dados, engenharia de atributos e ajuste de modelos, este projeto previu com sucesso o pouso do primeiro estágio do Falcon 9. Os insights obtidos são inestimáveis para estimar custos de lançamento e auxiliar empresas em suas licitações competitivas contra a SpaceX.

