# bitcoin-correlation
 Comparação e correlação do Bitcoin (BTC)  a vários indicadores financeiros, como o Ouro, o Índice S&P 500, o Índice do Dólar Americano e os rendimentos do Tesouro dos Estados Unidos de 5 anos e 10 anos. 

 O Bitcoin (BTC) é frequentemente comparado a vários indicadores financeiros, como o Ouro, o Índice S&P 500, o Índice do Dólar Americano e os rendimentos do Tesouro dos Estados Unidos de 5 anos e 10 anos. Essas comparações geralmente destacam a correlação ou correlação inversa entre o BTC e essas métricas, muitas vezes apoiadas por gráficos de movimento de preços. No entanto, a explicação matemática subjacente para essas correlações geralmente não é explorada. Para aprofundar esse tópico, realizamos uma análise abrangente para examinar a correlação entre o Bitcoin e essas métricas financeiras.

##### Visão geral do notebook:

In this notebook, we will conduct a correlation analysis between Bitcoin (BTC) and the following financial metrics:

* XAU - Ouro
* SPX - Índice S&P 500
* DXY - Índice do Dólar Americano
* FVX - Rendimento do Tesouro dos EUA de 5 anos
* TNX - Rendimento do Tesouro dos EUA de 10 anos

A análise será dividida nas seguintes seções:

* Coleta de dados
* Preparação dos dados
* Exploração dos dados
* Análise de correlação
* Visualização dos dados
* Interpretação e Conclusão


# Coleta de Dados

Os dados usados nesta análise são coletados do Yahoo Finance para o Bitcoin, os rendimentos do Tesouro e o S&P 500; e do Investing.com para o Índice do Dólar Americano e o Ouro. 
O intervalo de datas para os dados é de 17 de setembro de 2014 a 31 de maio de 2023.


### Análise de Regressão Linear

A regressão linear é uma técnica estatística utilizada para modelar a relação entre uma variável dependente e uma ou mais variáveis independentes. Ela pressupõe uma relação linear, permitindo-nos prever a variável dependente com base nas variáveis independentes.

Na nossa análise com BTC/SPX e BTC/XAU, realizamos uma regressão linear simples para entender a relação entre BTC (Bitcoin) e SPX (Índice S&P 500) e entre BTC e XAU (Ouro). Isso nos ajudou a avaliar a associação linear entre BTC e cada instrumento financeiro.

Para expandir nossa análise, exploramos a regressão linear múltipla. Ao considerar tanto XAU quanto SPX como variáveis independentes, previmos simultaneamente o BTC usando essas variáveis. Isso nos permitiu examinar como o preço do BTC é influenciado pelos efeitos combinados de XAU e SPX.

Os coeficientes obtidos a partir dos modelos de regressão representam a força e a direção da relação entre as variáveis independentes e BTC. Utilizamos esses coeficientes para criar um modelo preditivo que estima o preço do BTC com base nos valores de XAU e SPX.

Para visualizar os resultados da regressão, plotamos os preços reais do BTC ao lado dos preços do BTC previstos derivados dos modelos de regressão linear. Essa representação visual nos ajudou a avaliar a precisão dos modelos e obter insights sobre as relações entre BTC, XAU e SPX.

É importante observar que a regressão linear pressupõe linearidade entre as variáveis e determinadas suposições sobre os dados. Avaliar essas suposições e interpretar os resultados é crucial para obter conclusões confiáveis a partir da análise.

Ao focar em SPX e XAU, selecionamos instrumentos financeiros que possuem uma correlação positiva com o BTC. Essa escolha nos permitiu capturar as influências do mercado de ações mais amplo (SPX) e do mercado de metais preciosos (XAU) nos movimentos do preço do BTC. Além disso, nos ajudou a manter a análise focada e gerenciável, ao mesmo tempo em que fornecia insights significativos sobre as relações entre BTC e esses instrumentos-chave.

Por meio da aplicação de técnicas de regressão linear simples e múltipla, obtivemos insights sobre as associações entre BTC e instrumentos financeiros individuais (BTC/SPX, BTC/XAU) e os efeitos combinados de múltiplas variáveis (BTC/SPX,XAU) no preço do BTC.



# Conclusão

Nesta análise, exploramos a relação entre o Bitcoin e vários indicadores financeiros, incluindo Ouro, Índice S&P 500, Índice do Dólar Americano, Rendimento do Tesouro dos EUA de 5 anos e Rendimento do Tesouro dos EUA de 10 anos. Descobrimos que o Bitcoin possui uma forte correlação positiva com o Ouro e o Índice S&P 500, indicando que, à medida que o Ouro e o Índice S&P 500 aumentam, os preços do Bitcoin tendem a subir também. Por outro lado, o Bitcoin possui uma correlação negativa fraca com o Rendimento do Tesouro dos EUA de 10 anos e o Rendimento do Tesouro dos EUA de 5 anos, sugerindo que, à medida que os rendimentos desses títulos do Tesouro aumentam, os preços do Bitcoin podem sofrer uma leve diminuição.

Para avaliar a volatilidade e o risco sistemático do Bitcoin, calculamos o escore beta. O escore beta compara os movimentos de preço do Bitcoin com os de um benchmark, que no nosso caso foi o Índice S&P 500. O escore beta do Bitcoin em relação ao Índice S&P 500 foi de 17,29, indicando que o Bitcoin é significativamente mais volátil do que o mercado de ações em geral.

Realizamos análises de regressão linear e regressão linear múltipla para entender melhor as relações entre o Bitcoin e esses indicadores financeiros. A análise de regressão linear revelou a inclinação da relação entre o Bitcoin e cada indicador individualmente, enquanto a análise de regressão linear múltipla considerou várias variáveis simultaneamente para prever os preços do Bitcoin.

Essas descobertas fornecem insights valiosos para investidores e traders. A correlação positiva entre o Bitcoin e o Ouro, assim como o Índice S&P 500, sugere que o Bitcoin pode servir como uma potencial proteção contra a volatilidade do mercado e uma reserva de valor durante tempos econômicos incertos. No entanto, é importante observar que correlação não implica causalidade, e outros fatores também podem influenciar os preços do Bitcoin. Portanto, é essencial realizar pesquisas e análises adicionais antes de tomar decisões de investimento.

Vale ressaltar que os mercados financeiros são complexos e imprevisíveis, e o desempenho passado não é indicativo de resultados futuros. Portanto, é necessário um entendimento abrangente dos fatores subjacentes e uma avaliação de riscos completa ao considerar investimentos em Bitcoin ou qualquer instrumento financeiro.

Em geral, esta análise fornece uma base para entender as relações entre o Bitcoin e esses indicadores financeiros, oferecendo insights que podem informar estratégias de investimento e tomada de decisões.
