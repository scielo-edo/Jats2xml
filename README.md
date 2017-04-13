Descrição do projeto
=========

Command line
------------

*xml2tex* é um conversor de *xml jats* para ConTeXt, que 
segue as exigências do projeto SciELO.

Trata-se de uma aplicação de linha de comando que pode ser 
executada via *prompt*, podendo ser usado para 
a conversão de arquivos em massa, localmente, ou como 
parte integrada de qualquer aplicação.

```
xml2tex <Arquivo>.xml -o <Arquivo.tex>
```


O objetivo desse conversor é transformar as tags e os atributos do XML jats
para um padrão ConTeXt. Será possível escolher, um template de LaTeX diferente do *default*:

```
# uso com templates .tex
xml2tex <Arquivo>.xml -t <template> -o <Arquivo.tex>
```


Microservice
------------

O projeto inclui ainda um *microservice* ou servidor que 
recebe arquivos *xml* via *post* e devolve arquivos *.tex. 

Schemas
-------

O conversor pode servir ainda para outros esquemas de *xml* (*.xd). 
A correspondência entre os blocos de *xml* e os comandos *tex*
podem ser editados em uma aplicação *web* do tipo *admin*.

Tecnologia
==========

A aplicação deve fazer parte de um microsserviço *web* podendo ser 
integrada a qualquer outra aplicação para gerar arquivos *.tex a partir 
de XML. 

Avaliamos a possibilidade de tornar a aplicação compatível com o 
projeto de conversão chamado \textbf{pandoc}, mas só poderemos 
concluir se isto é possível após iniciarmos o desenvolvimento. 


Descrição do piloto
-------------------

Fizemos uma prova de conceito que pode ser acessada [neste endereço](beijaflor-jatex.herokuapp.com).




