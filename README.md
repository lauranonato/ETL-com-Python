Esse projeto tem como objetivo utilizar a linguagem de programação Python para realizar o processo de ETL - Extração, Transformação e Carregamento (Load) de diferentes formatos de arquivos (csv,Json,txt).
Foram transformados os dados, criados dataframes finais a partir desse processo, validados e carregados no banco de dados Big Query 

Fonte dos dados:

ETL de arquivo CSV: dados abertos de contratos administrativos da AEB - Agencia Espacial Brasileira 
https://dados.gov.br/dataset/dados-abertos-de-contratos-administrativos/resource/6a9526c4-bd86-46fb-b7aa-539df37f849a

ETL de arquivo JSON: dados abertos de contratos administrativos da AEB - Agencia Espacial Brasileira 
https://dados.gov.br/dataset/dados-abertos-de-recursos-humanos-da-aeb/resource/4ed1acb6-e403-4be5-8c8c-90b0248673d4?inner_span=True

ETL de arquivo TEXT: dados com historico de temperaturas medias diarias na cidade de Nova York de 1995 a 2020, disponibilizados pela Universidade Dayton
https://academic.udayton.edu/kissock/http/Weather/source.htm

Vale ressaltar que os dados estão na unidade de medida Fahrenheit e quando ha dados faltantes é adotado por default "-99"
Uma estrategia para tratar esse default foi substituir o "-99" por uma média da temperatura entre o dia anterior e o posterior (escolhendo o primeiro registro nao nulo desses)

Códigos desenvolvidos com o curso https://www.udemy.com/course/etl-basico-com-python/
