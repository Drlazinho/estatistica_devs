# Estatistica Dev Python

### Medidas.
- Medidas de Posição
    - media --> `mean()`
    - mediana --> `median()`
    - moda --> `mode()`
- Medidas de Dispersão
    - variança --> `var()`
    - desvio padrão --> `std()`
    - Coeficiente de Variação --> `std() / mean()`
- Medidas de Forma
    - Assimetria --> `skew()`
    - Curtose --> `kurtosis()`
- Medidas estatísticas --> `describe()`

### Correlação
- Correlação de Variáveis
    - Correlaçao do Dataframe, segundo Pearson --> `corr`(method='pearson')
    - Correlação entre 2 variaveis--> `corr(lista.segundaVariavel)`
    - Correlação do Dataframe, segundo Spearman --> `corr`(method='spearman')

### Graficas
- Histograma - `hist()`
- Gráfico de Barras Vertical --> `plot.bar(x='categorias', y='valor')`
- Grafico de Barras Vertical - Valor (ordenado) --> `df_vendas.sort_values('valor', ascending=False).plot.bar(x="categorias", y="valor")`
- Grafico de Barras HOrizontal --> `df_vendas.plot.barh(x='categorias', y='quantidade')`
- Grafico de Dispersão -->  `df_medidas.plot.scatter(x='idade', y='altura')`
- Grafico de BoxPlot (Diagrama de Caixa) --> `df_medidas.idade.plot.box()`
- Grafico de Linha --> `df_faturamento.plot.line(x='data_ref', y='valor')`

#### Informação dos tipos de dados
`.info()`

#### Conversão de dados
Convertendo dado de object para datetime
`df_faturamento.data_ref = pd.to_datetime(df_faturamento.data_ref)`
