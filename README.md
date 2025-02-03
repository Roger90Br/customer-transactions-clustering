# Análise de Comportamento de Clientes - Clusterização de Transações

Este projeto visa realizar uma análise aprofundada das transações de clientes de uma empresa utilizando técnicas de **clusterização** para identificar segmentos de comportamento, com base nas variáveis **Quantidade** e **Preço Unitário**. O objetivo é oferecer uma visão detalhada sobre os padrões de compra dos clientes e permitir uma segmentação eficaz para estratégias de marketing e vendas.

## Objetivo

O objetivo deste projeto é aplicar técnicas de **análise exploratória de dados (EDA)** e **clusterização** em dados de transações para:

- Identificar padrões de comportamento de compra.
- Agrupar os clientes em segmentos (clusters) com base em características similares.
- Utilizar a segmentação para informar decisões de marketing e personalização de ofertas.
- Explorar visualmente as distribuições e relações entre as variáveis.

## Dados

Os dados usados neste projeto são transações de clientes, com as seguintes variáveis principais:

- **Quantidade**: Número de itens comprados.
- **Preço Unitário**: Valor unitário dos itens comprados.
- **Código do Produto**: Identificação única de cada produto.
- **Data da Compra**: Data em que a transação ocorreu.

O objetivo é analisar o comportamento de compra, segmentando os clientes com base nas variáveis mencionadas.

## Etapas do Projeto

O projeto é composto pelas seguintes etapas:

### 1. Preparação dos Dados

- **Carregamento dos Dados**: O arquivo de transações é carregado e transformado em um DataFrame utilizando a biblioteca `pandas`.
- **Limpeza de Dados**: Os dados são tratados para lidar com valores nulos, dados duplicados e valores inconsistentes. Foi aplicada a normalização das variáveis para garantir que elas tenham a mesma escala.
- **Tratamento de Outliers**: A análise de outliers foi realizada para detectar e tratar possíveis valores anômalos nas variáveis de **Quantidade** e **Preço Unitário**.

### 2. Análise Exploratória de Dados (EDA)

Nesta fase, fizemos uma análise preliminar dos dados para entender as distribuições das variáveis e as relações entre elas. Alguns pontos abordados foram:

- Análise de dispersão entre **Quantidade** e **Preço Unitário**.
- Histograma da distribuição dos **Preço Unitário** e **Quantidade**.
- Identificação de correlações entre as variáveis.

### 3. Clusterização

A técnica de **clusterização** foi aplicada utilizando o algoritmo **K-Means**, com o objetivo de segmentar os clientes com base nas variáveis **Quantidade** e **Preço Unitário**. As etapas incluem:

- **Escolha do número de clusters**: Utilizamos o método do **Elbow** e o **Silhouette Score** para determinar o número ideal de clusters.
- **Treinamento do modelo**: O modelo K-Means foi treinado para formar clusters, com base nas variáveis selecionadas.
- **Análise dos clusters**: Cada cluster foi analisado para entender as características comuns de cada grupo.

### 4. Visualização

Após a clusterização, foram gerados gráficos para facilitar a interpretação dos resultados, incluindo:

- **Gráfico de dispersão** para visualizar os clusters.
- **Gráfico de Elbow** para determinar o número ideal de clusters.
- **Perfil dos clusters**: Tabelas e gráficos para descrever as características de cada grupo de clientes.

## Estrutura do Repositório

O repositório está organizado da seguinte forma:

