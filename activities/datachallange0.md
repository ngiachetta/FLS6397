# Introdução à Programação e Ferramentas Computacionais para as Ciências Sociais

- Autor: Leonardo S. Barone
- Adaptado por: Nathan Giachetta
- Data: definir

## Desafio 0

Siga as instruções abaixo. Documente __TODOS__ os seus passos em um script. Comente no seu script __TODOS__ os seus passos e explique a si mesm@ suas escolhas e estratégias. Colar pedaços de código nesta atividade é permitido e peça ajuda se precisar. Mencione __SEMPRE__ em comentários quando a solução encontrada não for sua.

1- Vá ao [Repositório de Dados Eleitorais do TSE](http://www.tse.jus.br/eleitor-e-eleicoes/estatisticas/repositorio-de-dados-eleitorais-1/repositorio-de-dados-eleitorais). Faça o download do arquivo de resultados de 2016 e descompacte-o. Você pode fazer tudo à mão se tiver dificuldade de copiar o modelo do [tutorial 4](https://github.com/ngiachetta/FLS6397/blob/master/tutorials/tutorial4.Rmd), em que abrimos os dados da MUNIC 2005. (Nome do arquivo: "VOTACAO EM __PARTIDO__ POR MUNICÍPIO E ZONA")

2- Importe para o R os resultados eleitorais dos 3 estados do Sul.

3- Com a função _rbind_ (ou bind_rows do pacote dplyr), junte os 3 _data frames_ importados.

4- Leia até o final as instruções deste desafio e identifique quais variáveis são necessárias para tarefa. Selecione apenas tais variáveis e renomeia-as (você pode trocar a ordem se achar mais fácil).

5- Selecione apenas as linhas que contém resultados eleitorais para prefeit@.

6- Selecione apenas as linhas que contém os resultados eleitorais para prefeit@s com votação nominal maior do que 10000 votos.

7- Quantas linhas restaram? Quantas colunas? 

### Bônus

8- Crie, a seu critério, 3 categorias de partido e crie uma nova variável: esquerda, direita, irrelevantes. Dê o nome de partido\_categoria a esta variável.

8- Faça uma tabela da nova variável.
