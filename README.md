<h2 align="center"> Análise de Gastos de Operadoras de Plano de Saúde </h2>
<h5 align="right"> Projeto I </h5>
<h5 align="right"> Representação do laboratório proposto pela DSA </h5>
<h5 align="right"> Microsoft Power BI para Data Science Versão 2.0 </h5>

*Situação hipotética: Quinta-feira, 12, 18:00h*

*Reunião multidisciplinar*|
------------------------- | 
*Assunto*                 |
*Encontrar alternativas para monitorar a evolução dos gastos já que estes aumentaram de forma considerável. Ideias, anotações, opniões, críticas serão postas para análise.*

Durante a reunião, os diretores fizeram diversas perguntas aos presentes (gestores e profissionais de TI e BI), e após o encontro, a equipe elencou o que precisa de fato ser considerado para monitorar os gastos da empresa:

#### Fatores/Requisitos:
- [ ] Gasto total da operadora;
- [ ] Idade média dos usuários da operadora;
- [ ] Gasto médio por região;
- [ ] Faixa etária com maior gasto com seguro saúde por região;
- [ ] A relação de filhos com o gasto;
- [ ] Proporção de crianças por região;
- [ ] A relação de idade com o IMC;
- [ ] Que gênero gasta mais.

Além disso, duas situações:
- [ ] Se o usuário for mulher, o imc é acima ou abaixo da média? Compare pela faixa etária.
- [ ] Se for homem, na faixa de 20 a 59 anos e da região Sudeste, o gasto é maior ou menor que a média de gastos da região?

O CEO, por fim, diz:
> _ Você, o analista de dados, preciso de um dashboard interativo de única tela onde pudesse visualizar todos nossos requisitos a qualquer momento;

> _ Precisa ser capaz de monitorar e relacionar os dados. Quero poder descobrir os problemas e as oportunidades a partir desses dados.

#### Pontos dignos de nota do dashboard:

- [X] A relação de filhos com o gasto;
<p align="justify"> Sem nenhuma informação extra informada, pude classificá-los para os que possuem filhos de "Pais" e sem filhos de "Sem filhos". Então, a porcentagem obtida não foi com relação ao número de filhos, e sim compara a variação dos gastos para aqueles que têm filhos ou não. Um filtro poderia ser inserido para comparar os gastos dos "Sem filhos" com uma quantidade específica de filhos, mas a decisão cabe ao tomador de decisão. </p>

<p align="center"> <img src="https://github.com/diogogon/projeto-1/blob/main/Text.png">

- [X] Se o usuário for mulher, o imc é acima ou abaixo da média? Compare pela faixa etária.
- [X] Se for homem, na faixa de 20 a 59 anos e da região Sudeste, o gasto é maior ou menor que a média de gastos da região?

Para demonstrar essas situações hipotéticas foi proposto KPI's interativos, que tomam como ponto de partida a média total de cada requisito (IMC e gastos) travado às variáveis:
1. Requisito gastos: a média de gastos total está travada por **gênero** e **região**. O que significa que esses dois filtros não alteram a média de gastos total. Outro filtro como o de faixa etária, por exemplo, já altera o valor de comparação.
2. Requisito IMC: a média de gastos total está travada por **gênero** e **faixa etária**.

*Os valores travados foram intencionais para análise.*

Por fim, as opções de filtro tornam possíveis análises por gênero, região e faixa etária dependendo de cada caso.

<p align="center"> <img src="https://github.com/diogogon/projeto-1/blob/main/KPI_IMC.png"> <img src="https://github.com/diogogon/projeto-1/blob/main/KPI_Gasto.png">

<p align="justify"> Para os outros requisitos, não há qualquer dificuldade na construção dos gráficos. Houve apenas um cuidado a mais em *como* construir os gráfico e organizar no dashboard. Marcadores, cores, escolha apropriada dos gráficos, saturação, o modo de visualização e interação, e filtros. Uma história ainda pode ser contada por dashboard sem relação com um período contínuo de data? Claro que sim, e é dessa forma que é apresentado aos diretores. </p>

O dashboard completo pode ser visto a seguir:

<p align="center"> <img src="https://github.com/diogogon/projeto-1/blob/main/Visual_geral.png">

O arquivo .pbix do dashboard:
[projeto I PBI: Análise de gastos na saúde](https://github.com/diogogon/projeto-1/blob/main/projeto-1.pbix)

#### Bibliografia
O arquivo original do dataset .csv mais o desafio proposto estão no curso gratuito Microsoft Power BI para Data Science Versão 2.0 oferecido pela DSA. Os arquivos originais são postos de maneira didática e há problemas propositais que simulam a vida real do profissional. Apoie o trabalho.

*OBS: Minha solução já está com todas as modificações que eu julgo correta para a análise dos dados, tanto o dataset como o problema.*

#### Autor
*Diogo Gonçalves*
> E-mail: dio.goncalves90@gmail.com

> Github: https://github.com/diogogon

> Linkedin: www.linkedin.com/in/diogogon
