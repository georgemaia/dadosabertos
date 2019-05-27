# Guia Biblioteca Pandas

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



**Exibir a quantidade de empresas únicas**

*empresas = df['Empresa'].unique()*

*len(empresas)*





## Referências

[https://github.com/reisdebora/analisapenalidadesCNPJ/blob/master/analisa_penalidades.md](https://github.com/reisdebora/analisapenalidadesCNPJ/blob/master/analisa_penalidades.md)

[https://github.com/alvarofpp/analise-ufrn-python-day-2018](https://github.com/alvarofpp/analise-ufrn-python-day-2018)

[https://github.com/aguinaldoabbj/minicourse_open_data_natal_2019](https://github.com/aguinaldoabbj/minicourse_open_data_natal_2019)

https://github.com/leportella/datascience-pizza](https://github.com/leportella/datascience-pizza)
