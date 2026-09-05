**Aerosol Transport — Análise do Transporte Atmosférico de Aerossóis**

🇺🇸 [English Version](README.md)

**Visão Geral**

Pipeline de dados desenvolvido em Python para integração, processamento e análise de aerossóis atmosféricos, variáveis meteorológicas e observações de queimadas sobre a América do Sul.

O projeto investiga a evolução espacial e vertical dos aerossóis atmosféricos por meio da combinação de dados atmosféricos tridimensionais com observações de queimadas, estabelecendo uma estrutura para análise do transporte de aerossóis e modelagem preditiva.

**Problema**

Emissões provenientes de queimadas podem ser transportadas por grandes distâncias e atingir diferentes níveis da atmosfera dependendo das condições meteorológicas.

Compreender essa evolução exige a integração de diferentes fontes de informação atmosférica, incluindo concentrações de aerossóis, variáveis meteorológicas, níveis de pressão e observações de queimadas.

Este projeto busca processar e integrar esses conjuntos de dados multidimensionais em uma estrutura espaço-temporal consistente para análise do transporte atmosférico de aerossóis.

**Solução**

Foi desenvolvido um workflow em Python para integrar dados atmosféricos e de queimadas e analisar a evolução horizontal e vertical dos aerossóis.

O processamento inclui:

* processamento de dados atmosféricos multidimensionais;
* integração de variáveis meteorológicas e de aerossóis;
* integração de observações de queimadas;
* análise em diferentes níveis atmosféricos;
* geração de perfis verticais de aerossóis;
* análise espacial e temporal das concentrações;
* construção de datasets estruturados para modelagem preditiva;
* visualização do transporte horizontal e vertical dos aerossóis.

## 🗂️ Dados

**MERRA-2**

Dados de reanálise atmosférica utilizados para obtenção de variáveis meteorológicas e de aerossóis em diferentes níveis verticais.

Entre as variáveis analisadas estão espécies de aerossóis como:

* Carbono Orgânico (OC);
* Black Carbon (BC);
* propriedades ópticas dos aerossóis;
* variáveis meteorológicas relacionadas ao transporte atmosférico.

**FIRMS**

Observações de queimadas derivadas de satélite utilizadas para caracterizar espacial e temporalmente a ocorrência de fogo.

Os dados brutos não estão incluídos neste repositório devido ao seu volume.

**Metodologia**

O fluxo geral de processamento segue:

**Dados Atmosféricos → Pré-processamento → Integração com Queimadas → Análise Vertical → Dataset Espaço-Temporal → Análise de Transporte → Modelagem Preditiva**

O pipeline organiza as variáveis atmosféricas no espaço, no tempo e em diferentes níveis verticais, permitindo investigar as relações entre condições meteorológicas, ocorrência de queimadas e evolução dos aerossóis.

**Modelagem Preditiva**

O projeto fornece uma estrutura para investigar se o estado atual da atmosfera pode ser utilizado para estimar o comportamento subsequente dos aerossóis.

O dataset de modelagem combina concentrações de aerossóis, condições meteorológicas, informações de queimadas e estrutura vertical da atmosfera para experimentos de Machine Learning voltados à evolução dos aerossóis.

Esta componente encontra-se em desenvolvimento.

**Produtos Gerados**

O workflow permite gerar:

* mapas de concentração de aerossóis;
* perfis verticais;
* séries temporais;
* comparações entre níveis atmosféricos;
* datasets espaço-temporais de aerossóis;
* visualizações da evolução horizontal e vertical dos aerossóis.

**Tecnologias**

* Python
* Xarray
* NumPy
* Pandas
* SciPy
* Matplotlib
* Cartopy
* NetCDF
* MERRA-2
* FIRMS
* Machine Learning

**Estrutura do Projeto**

```text
Aerosol_Transport/
│
├── README.md
├── README_PT.md
├── requirements.txt
│
├── src/
│   ├── data_processing.py
│   ├── fire_processing.py
│   ├── vertical_analysis.py
│   ├── transport_analysis.py
│   ├── feature_engineering.py
│   └── visualization.py
│
└── figures/
```

**Status do Projeto**

Em desenvolvimento ativo.

O trabalho atual está concentrado na integração dos dados atmosféricos, análise vertical dos aerossóis e desenvolvimento dos datasets utilizados na modelagem preditiva.

**Autor**

**Paulo Antunes**

Meteorologista | Cientista de Dados Atmosféricos | Desenvolvimento de Produtos de Dados & IA
