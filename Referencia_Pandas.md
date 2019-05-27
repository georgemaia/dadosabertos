# Biblioteca Pandas

**Carregar a biblioteca Pyhton Panda**

*import pandas as pd*

**Baixar o arquivo CSV**

*wget - c URL*

Sendo a URL o endereço do arquivo

**Carregar o arquivo CSV**

*df = pd.read_csv("FILE", enconding='iso-8859-1', sep = ';', thousands=r'.')_*

Sendo FILE o nome do arquivo baixado, o separador dos registros sendo o ; e o indicativo de milhar o ponto.

**Checar se o arquivo foi carregado**

*df.head()*

Exibe os primeiros registros

**Exibir os últimos registos**

*df.tail()*

**Exibir 10 registros aleatórios**

*df.sample(10)*

**Exibir o número de linhas e colunas**

*df.shape*

**Exibir informações do dataset como nome da coluna, tamanho e tipo de valores**

*df.info()*

**Exibir informações estatísticas das colunas numéricas**

*df.describe()*

count: número total; 

mean: média; 

std:desvio padrão; 

min: valor mínimo; 

25%: quartil 25%; 

50%:quartil 50% ; 

75%:quartil 75% ; 

max: valor máximo;

**Exibir tipos de dados das colunas**

*df.dtypes*

**Exibir a sétima linha**

*df.loc[6]*

**Exibir as linhas a partir da 4 até a 8**

*df.loc[3:7]*

**Exibir as linhas 2, 5 e 10**

*df.loc[[1,4,9]]*

**Exibir as linhas da empresa específicas**

*df[df['Empresa'] == "CONCEIÇÃO"].head()*

**Exibir coluna individual**

*df['Empresa']*.head()

**Exibir as colunas**

df.columns

**Exibir a quantidade de empresas únicas**

*empresas = df['Empresa'].unique()*

*len(empresas)*

**Selecionar Multiplas colunas pelo nome**

*df[['Empresa','Linha']].head()*

**Apagar Colunas**

*df.drop(['Estudante_Cartao_', 'Estudante_BT'], axis=1).head()*

axis=1 significa através de colunas

**Exibir apenas algumas colunas**

*df.drop(df.columns.difference(['Mês','Empresa','Qtd_Viagens']), axis=1).head()*

**Adicionar Colunas Calculadas**

*df['Integracao_Total'] = df['Integracao_Plena' + df['Integracao_Complementar']]*

*df.sample(5)*

**Converter tipo de coluna**

*df["Linha"] = df["Linha"].astype(str)*

Converter a coluna Linha de int64 para string

**Método para converter número do mês em extenso**

*from calendar import month_name #importa apenas o nome do mes da biblioteca calendar*

month_names = df.Mês.apply(lambda x: month_name[x])

**Exibe o nome do mês**

*month_name[3]*

**Adiciona nova comluma chamada Month**

*df['Month'] = month_names*

*df.head()*

**Classificar pela coluna do dataset**

*df.sort_values("Qtd_Viagens_", ascending=False)*

**Classificar mais de uma coluna do dataset**

*df.sort_values(by=['Estudante_Cartao', 'Estudante_BT'], ascending=False).head(10)*

**Agrupando informações em coluna**

*df.groupby(['Month','Mês'], as_index=False).sum()*

Agrupa as colunas pelo mês

## Referências

[https://github.com/reisdebora/analisapenalidadesCNPJ/blob/master/analisa_penalidades.md](https://github.com/reisdebora/analisapenalidadesCNPJ/blob/master/analisa_penalidades.md)

[https://github.com/alvarofpp/analise-ufrn-python-day-2018](https://github.com/alvarofpp/analise-ufrn-python-day-2018)

[https://github.com/aguinaldoabbj/minicourse_open_data_natal_2019](https://github.com/aguinaldoabbj/minicourse_open_data_natal_2019)

[https://github.com/leportella/datascience-pizza](https://github.com/leportella/datascience-pizza)
