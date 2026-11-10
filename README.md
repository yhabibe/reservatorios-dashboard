# Reservatórios do SIN

Painel interativo de armazenamento (EAR) e afluência (ENA) do Sistema Interligado Nacional, com dados do ONS e classificação ENSO baseada no ONI da NOAA.

**[Abrir o painel](https://yhabibe.github.io/reservatorios-dashboard/)**

Compare anos para o SIN, subsistemas, bacias e Reservatórios Equivalentes de Energia (REEs).

O arquivo `index.html` contém os dados e a biblioteca de gráficos ECharts e também pode ser baixado e aberto offline.

## Atualização

Esta publicação é uma fotografia dos dados, com referência em **08/11/2026**. Não há atualização automática das fontes.

Para publicar uma nova versão, gere novamente `dados_ons/dashboard.html` no projeto de origem, copie seu conteúdo para `index.html` neste repositório e envie um commit para `main`. O GitHub Pages publica a alteração automaticamente.

## Fontes

- [Dados abertos do ONS](https://dados.ons.org.br/)
- [Oceanic Niño Index — NOAA/CPC](https://www.cpc.ncep.noaa.gov/data/indices/oni.ascii.txt)
- [Apache ECharts](https://echarts.apache.org/)

Este repositório contém apenas o painel publicado.
