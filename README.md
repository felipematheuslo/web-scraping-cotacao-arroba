## Sobre o script
Script desenvolvido em python com o propósito de obter as cotações atuais do boi gordo e da vaca gorda de cada cidade (em R$/arroba) utilizando a técnica de _web scraping_, e salvar em um arquivo .csv para registro histórico. Tais informações são disponibilizadas aos produtores na página _web_ [Scot Consultoria](https://www.scotconsultoria.com.br/cotacoes)

- A bilbioteca `Selenium` foi utilizada para acessar a página _web_ e realizar a captura do elemento html no qual se encontram os dados.
- A biblioteca `Beautiful Soup` foi utlizada para extrair os dados contidos dentro desse elemento html.
- A bilbioteca `Pandas` foi utlizada para limpar, manipular e estruturar os dados obtidos.

Com o _data frame_ montado da forma desejada, o script adiciona a cotação atual em seu respectivo arquivo.

## Saída esperada
### cotacao_boi_gordo.csv
```
data,região,à vista,30 dias
10/05/2022,SP Barretos,306.5,308.5
10/05/2022,SP Araçatuba,306.5,308.5
10/05/2022,MG Triângulo,288.5,290.5
11/05/2022,SP Barretos,305.5,307.5
11/05/2022,SP Araçatuba,305.5,307.5
11/05/2022,MG Triângulo,283.5,285.5
12/05/2022,SP Barretos,305.5,307.5
12/05/2022,SP Araçatuba,305.5,307.5
12/05/2022,MG Triângulo,282.5,284.5
```
### cotacao_vaca_gorda.csv
```
data,região,à vista,30 dias
data,região,à vista,30 dias
10/05/2022,SP Barretos,273.0,275.0
10/05/2022,SP Araçatuba,273.0,275.0
10/05/2022,MG Triângulo,254.0,256.0
11/05/2022,SP Barretos,272.0,274.0
11/05/2022,SP Araçatuba,272.0,274.0
11/05/2022,MG Triângulo,254.0,256.0
12/05/2022,SP Barretos,272.0,274.0
12/05/2022,SP Araçatuba,272.0,274.0
12/05/2022,MG Triângulo,254.0,256.0
```
