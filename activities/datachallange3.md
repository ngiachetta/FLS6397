# Introdução à Programação e Ferramentas Computacionais para as Ciências Sociais

- Responsável: Leonardo S. Barone
- Adaptado por: Nathan Giachetta
- Data: definir

## Desafio 3

## Instruções para Entrega

Data: definir

Formato: 2 arquivos: (1) RScript (arquivo .R); (2) arquivo .pdf ou .html produzido com RMarkdown.

Atualização: se você perdeu a apresentaçãosobre RMarkdown, recomendo ler o curto capítulo [_R Markdown basics](http://r4ds.had.co.nz/r-markdown.html#r-markdown-basics) do livro _R for Data Science_ sobre o tema. Se você tiver problema com o RMarkdown, pode me entregar apenas um script.

Via: e-mail com título "[R-CiênciasSociais] - D3".

__OBS: VOCÊ PODE FAZER ESTA ATIVIDADE SOZINH@ OU EM GRUPO DE ATÉ 3 PESSOAS__

## Instruções para a atividade

Siga as instruções abaixo. Faça no arquivo de RMarkdown uma síntese de sua atividade e apresente apenas o essencial do código (você deve julgar o que é essencial).

Documente __TODOS__ os seus passos no arquivo de script. Comente no seu script __TODOS__ os seus passos e explique a si mesm@ suas escolhas e estratégias.

O arquivo .pdf ou .html produzido em RMarkdown deve contar as informações dos integrantes do grupo.

As primeiras linhas do seu script devem conter suas informações pessoais como comentário, tal qual o modelo abaixo:

```{r}
### nome <- c("Fulano da Silva Sauro","Fulana da Silva Sauro","Sauro da Silva Fulano")
### graducao <- c("Primeiro ano", "Segundo ano", "Quarto ano")
### n_usp <- c(32165438,78165598, 43895498)
### data_entrega: ""
```

### Parte 1 - Combinando fontes de dados diferentes

Construa um data frame com as seguintes características: as observações devem ser municípios e as colunas características dos municípios;

Você deve construir esse data frame combinando as seguintes fontes:

- [Perfil dos Municípios Brasileiros 2015](http://www.ibge.gov.br/home/estatistica/economia/perfilmunic/2015/default.shtm) - Bases de dados em .xls no menu do lado esquerdo
- [Informações Financeiras e Fiscais dos Municípios](https://siconfi.tesouro.gov.br/siconfi/pages/public/consulta_finbra/finbra_list.jsf)
- [Estatísticas sobre óbitos - DATASUS](http://tabnet.datasus.gov.br/cgi/deftohtm.exe?sim/cnv/pobt10br.def)
- Outra fonte de sua escolha.

Para os que tiverem dificuldades com as bases de dados, utilize as cópias que deixei no repositório: [MUNIC15](https://github.com/ngiachetta/FLS6397/blob/master/data/Base_MUNIC_2015_xls.zip?raw=true), [DATASUS](https://raw.githubusercontent.com/ngiachetta/FLS6397/master/data/obitos_datasus.csv) e [FINBRA](https://github.com/ngiachetta/FLS6397/blob/master/data/receitas_orc_finbra.zip?raw=true)

Lembre-se que as bases devem ser combinadas utilizando o código de município. Algumas fontes podem contar códigos com 6 ou 7 dígitos e você deve ignorar o 7o dígito se isso ocorrer.

Para tranformar um código de 7 dígitos em um de 6 dígitos faça:

```{r setup, include=FALSE}
cod_ibge6 <- as.numeric(substr(cod_ibge7, 1, 6))
```

Escolha as variáveis de seu interesse em cada fonte e mantenha apenas estas no data frame.

### Parte 2 - Análise exploratória e gráfica dos dados

Utilizando os capítulos [Cap 3. Visualização de dados](http://r4ds.had.co.nz/data-visualisation.html) e [Cap 7. Análise exploratória de dados](http://r4ds.had.co.nz/exploratory-data-analysis.html), faça uma apresentação criativa dos dados e explore relações entre variáveis das diversas fontes.
