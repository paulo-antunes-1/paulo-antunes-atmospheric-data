**S2S Brazil — Verificação de Previsões Subsazonais**

Sistema para processamento, avaliação e visualização do desempenho de previsões subsazonais de temperatura sobre o Brasil utilizando os modelos CESM e E3SM e dados de referência ERA5-Land.

**Problema:**

Previsões subsazonais buscam preencher a lacuna entre a previsão meteorológica de curto prazo e a previsão climática sazonal.

Este projeto avalia a capacidade de modelos climáticos em representar a variabilidade da temperatura sobre diferentes regiões do Brasil em horizontes subsazonais, com foco nas previsões Week 3 e Week 3–4.

**Solução:**

Foi desenvolvido um pipeline em Python para processamento e avaliação das previsões, incluindo:

- leitura e processamento de dados climáticos em NetCDF;
- processamento das previsões CESM e E3SM;
- utilização do ERA5-Land como referência;
- cálculo de métricas de desempenho;
- avaliação espacial das previsões;
- análise das cinco regiões brasileiras;
- comparação do desempenho entre os modelos;
- geração automatizada de mapas e gráficos.

**Dados:**

**Modelos:**

- CESM
- E3SM

**Referência:**

- ERA5-Land

Os arquivos brutos não estão incluídos neste repositório devido ao volume dos conjuntos de dados.

**Métricas:**

O desempenho das previsões é avaliado utilizando métricas como:

- Anomaly Correlation Coefficient (ACC);
- percentual de previsões com ACC > 0,5;
- métricas regionais de desempenho.

As análises são realizadas para:

- Norte;
- Nordeste;
- Centro-Oeste;
- Sudeste;
- Sul.

**Tecnologias:**

- Python
- Xarray
- NumPy
- Pandas
- Matplotlib
- Cartopy
- GeoPandas
- NetCDF

Estrutura do projeto: 

```text
S2S_Brazil_Forecast_Verification/
│
├── README.md
├── requirements.txt
│
├── src/
│   ├── data_processing.py
│   ├── forecast_verification.py
│   ├── regional_analysis.py
│   └── visualization.py
│
├── figures/
│
└── app/
    └── app.py
```

**Resultados:** 

Os resultados mostram diferenças espaciais importantes na previsibilidade subsazonal da temperatura sobre o Brasil.

De maneira geral, os maiores valores de ACC são observados nas regiões Sul, Nordeste e Sudeste, enquanto a Região Norte apresenta menor previsibilidade.

### Desempenho regional

| Região       | CESM ACC médio | E3SM ACC médio | CESM ACC > 0,5 | E3SM ACC > 0,5 |
| ------------ | -------------: | -------------: | -------------: | -------------: |
| Sul          |          0,788 |          0,737 |          92,3% |          86,5% |
| Nordeste     |          0,742 |          0,624 |          85,5% |          69,7% |
| Sudeste      |          0,720 |          0,682 |          85,8% |          83,1% |
| Centro-Oeste |          0,646 |          0,580 |          79,0% |          67,4% |
| Norte        |          0,358 |          0,318 |          30,3% |          28,9% |

**Produto:**

O projeto está sendo desenvolvido como um dashboard interativo para exploração do desempenho das previsões subsazonais sobre o Brasil.

A aplicação permitirá selecionar regiões, modelos e métricas e visualizar os resultados de forma interativa.

**Dashboard:** Em desenvolvimento.

**Autor:**

**Paulo Antunes**

Meteorologista | Cientista de Dados Atmosféricos | Desenvolvimento de Produtos de Dados & IA
