Frete, Distância e Receita: O Impacto Logístico por Região



Tech Challenge — Fase 1 | POSTECH DTAT



\---



Sobre o Projeto



Este projeto analisa como as diferenças geográficas influenciam os custos de frete e a geração de receita no e-commerce brasileiro. A ideia central é entender se estados mais afastados dos grandes centros de distribuição pagam fretes proporcionalmente mais altos e, se sim, o quanto isso pesa na receita do marketplace.



Além da distância, fatores como pedágios, combustível, manutenção de frota e dificuldades de acesso variam bastante entre as regiões e contribuem para esse desequilíbrio logístico.



\---



Objetivos



\- Mapear a distribuição geográfica dos clientes por região

\- Identificar a relação entre distância dos centros de distribuição e custo de frete

\- Medir o impacto do frete na receita gerada por região

\- Propor ações para reduzir os gargalos logísticos identificados



\---



Principais Descobertas



1. Clientes concentrados no Sul e Sudeste

A base de clientes está fortemente concentrada nessas duas regiões, com São Paulo liderando o volume. Norte, Nordeste e Centro-Oeste ficam bem atrás, não por falta de demanda, mas pelas barreiras logísticas que encarecem o acesso ao marketplace.



2. Quanto mais longe, mais caro o frete

A análise confirma que as regiões mais distantes dos centros de distribuição do Sudeste pagam fretes significativamente mais altos. Norte e Nordeste são os casos mais críticos.



3. Frete alto, receita baixa

O Sudeste tem o menor frete médio e concentra a maior fatia da receita total. O Norte tem o maior custo de frete e a menor contribuição para o faturamento. Essa relação inversa aparece de forma clara nos dados.



\---



Ferramentas e Tecnologias



| Ferramenta | Uso |

|---|---|

| Power BI | Visualização de dados e criação dos dashboards |

| DAX | Medidas e colunas calculadas |

| Power Query | Transformação e limpeza dos dados |

| Dataset Olist | Fonte dos dados de e-commerce brasileiro |



\---



Expressões DAX Criadas



Foram criadas 11 expressões DAX ao longo da análise, entre colunas calculadas e medidas:



| # | Nome | Tabela | Tipo |

|---|---|---|---|

| 01 | Região | Lista de Clientes | Coluna Calculada |

| 02 | Nome do Estado | Lista de Clientes | Coluna Calculada |

| 03 | Ordem Região | Lista de Clientes | Coluna Calculada |

| 04 | Valor do Frete R$ | Itens do Pedido | Coluna Calculada (Power Query) |

| 05 | Preço do Item R$ | Itens do Pedido | Coluna Calculada (Power Query) |

| 06 | Total Pedidos | Itens do Pedido | Medida DAX |

| 07 | Receita Total | Itens do Pedido | Medida DAX |

| 08 | Frete Médio por Região | Itens do Pedido | Medida DAX |

| 09 | Frete Médio R$ | Itens do Pedido | Medida DAX |

| 10 | Total Clientes por Estado | Lista de Clientes | Medida DAX |

| 11 | Frete Médio Norte | Itens do Pedido | Medida DAX |



> A documentação completa de cada expressão está em \[`Documentação\_DAX.docx`](./Documentação\_DAX\_.docx)



\---



 Estrutura do Repositório



```

tech-challenge-fase1/

├── Tech\_Challenge\_Insight\_6.pbix          # Dashboard Power BI

├── Relatório\_Frete\_Distância\_Receita.docx # Relatório analítico completo

├── Documentação\_DAX.docx                  # Documentação das expressões DAX

└── README.md

```



\---



Visualizações do Dashboard



O dashboard no Power BI é composto por três gráficos principais:



Gráfico 1 — Distribuição Geográfica dos Clientes: Mapa de formas dos estados brasileiros colorido pela densidade de clientes

Gráfico 2 — Frete Médio por Região: Barras horizontais com o frete médio por pedido em cada região

Gráfico 3 — Frete Médio vs Receita por Região: Gráfico de linhas cruzando as duas métricas para mostrar a relação entre custo logístico e receita



\---



Recomendações



Dois caminhos principais para reduzir os gargalos e ampliar a receita nas regiões menos atendidas:



1. Expandir a infraestrutura logística

Criar hubs ou pontos de apoio no Norte e Nordeste para encurtar distâncias e reduzir o custo e o prazo das entregas.



2. Fortalecer sellers regionais

Incentivar vendedores locais a entrar na plataforma, reduzindo a dependência de envios que partem do Sudeste.



\---



Fonte de Dados



\- OLIST. Brazilian E-Commerce Public Dataset. Kaggle, 2024. Disponível em: \[https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

\- DATA FRETE. Composição do valor do frete. 2024. Disponível em: \[https://www.datafrete.com/valor-do-frete/](https://www.datafrete.com/valor-do-frete/)



\---



Autoria



Desenvolvido como parte do Tech Challenge — Fase 1 da Pós-Graduação em Data Analytics (POSTECH DTAT).

