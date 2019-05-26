# Guia inicial

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

## Referências

[https://github.com/reisdebora/analisapenalidadesCNPJ/blob/master/analisa_penalidades.md](https://github.com/reisdebora/analisapenalidadesCNPJ/blob/master/analisa_penalidades.md)

[https://github.com/alvarofpp/analise-ufrn-python-day-2018](https://github.com/alvarofpp/analise-ufrn-python-day-2018)

[https://github.com/aguinaldoabbj/minicourse_open_data_natal_2019](https://github.com/aguinaldoabbj/minicourse_open_data_natal_2019)

Guia do cientista de dados: [https://github.com/leportella/datascience-pizza](https://github.com/leportella/datascience-pizza)