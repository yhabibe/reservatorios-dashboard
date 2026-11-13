# Reservatórios do SIN

Painel público de energia armazenada (EAR), energia natural afluente (ENA), bandeiras tarifárias e Preço de Liquidação das Diferenças (PLD), com dados do ONS, da ANEEL e da CCEE e classificação ENSO baseada no ONI da NOAA.

**[Abrir o painel](https://yhabibe.github.io/reservatorios-dashboard/)**

Compare anos para o SIN, subsistemas, bacias e Reservatórios Equivalentes de Energia (REEs). O arquivo `index.html` contém os dados e a biblioteca ECharts e pode ser baixado e aberto offline.

## Conteúdo

- EAR diária, ENA mensal e mapa de calor da EAR, com comparação entre anos e contexto ENSO.
- Calendário das bandeiras tarifárias, com adicionais históricos publicados pela ANEEL.
- PLD médio mensal oficial dos quatro submercados da CCEE.
- Indicador analítico **SIN — PLD médio ponderado pela carga**, com pesos mensais do ONS e tabela de metodologia e pesos.

## Referências desta publicação

Atualizado em **13/11/2026**:

- Reservatórios: referência ONS em **11/11/2026**.
- Bandeiras: janeiro/2015 a novembro/2026.
- PLD regional: janeiro/2001 a outubro/2026, com 1.240 registros nos quatro submercados.
- PLD ponderado do SIN: 307 meses entre janeiro/2001 e outubro/2026. Dezembro/2013, fevereiro/2014 e abril/2015 permanecem sem indicador por cargas diárias ausentes no ONS.

## Metodologia do PLD ponderado

Em cada mês, o peso de um subsistema é sua participação na carga mensal dos quatro subsistemas. A carga mensal é calculada a partir de todos os dias do mês. O indicador resulta da soma dos PLDs médios mensais regionais multiplicados por esses pesos. O cálculo preserva a precisão e arredonda apenas a exibição.

Somente meses completos, com carga e preço dos quatro subsistemas, são calculados. Não há interpolação, uso de pesos antigos ou renormalização com regiões faltantes.

Esse indicador é uma agregação analítica para o painel. Não substitui os PLDs oficiais regionais, não reproduz uma ponderação horária de preços e consumo e não representa a tarifa final ao consumidor. Os preços são nominais, sem correção pela inflação. A carga ONS tem mudanças de abrangência em março/2021 e desde 29/04/2023, documentadas no painel.

## Atualização

A publicação é uma fotografia dos dados. Abrir o painel não consulta nem atualiza as fontes.

Para publicar uma nova versão, gere `dados_ons/dashboard.html` no projeto de origem, copie seu conteúdo para `index.html` neste repositório e envie um commit para `main`. O GitHub Pages publica a alteração automaticamente.

## Fontes

- [ONS — dados abertos](https://dados.ons.org.br/)
- [ONS — carga de energia diária](https://dados.ons.org.br/dataset/carga-energia)
- [ANEEL — bandeiras tarifárias](https://dadosabertos.aneel.gov.br/dataset/bandeiras-tarifarias)
- [CCEE — PLD média mensal](https://dadosabertos.ccee.org.br/dataset/pld_media_mensal)
- [NOAA/CPC — Oceanic Niño Index](https://www.cpc.ncep.noaa.gov/data/indices/oni.ascii.txt)
- [Apache ECharts](https://echarts.apache.org/)

Atribuição dos dados às respectivas fontes. ONS: CC BY; CCEE: CC BY 4.0; ANEEL: ODbL, conforme os catálogos. Transformações aplicadas: padronização de datas e códigos, consolidação das séries, agregação mensal da carga e derivação do PLD ponderado. Este repositório contém o painel publicado e sua documentação.
