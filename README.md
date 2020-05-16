[English Version](en/README.md)

# Sistemas de Banco de Dados
Este &eacute; um conjunto de palestras e materiais sobre sistemas de banco de dados provendo uma introdu&ccedil;&atilde;o aos principais m&eacute;todos e algoritmos usados para armazenamento e recupera&ccedil;&atilde;o de dados, especialmente os usados em sistemas gerenciadores de banco de dados tradicionais.

## Introdu&ccedil;&atilde;o
Sistemas de banco de dados referem-se ao conjunto de dados relacionados e sua respectiva forma de acesso e organiza&ccedil;&atilde;o. Formalmente, eles s&atilde;o compostos por uma cole&ccedil;&atilde;o de dados organizados (banco de dados), uma estrutura l&oacute;gica dos dados determinando a forma como podem ser armazenados, organizados e manipulados (modelo de dados), e um software que prov&ecirc; acesso ao banco de dados a usu&aacute;rios e aplica&ccedil;&otilde;es (sistema gerenciador de banco de dados) \[[2](#Elmasri-2016-BOOK)\].

Sistemas de banco de dados relacionais utilizam um modelo de dados relacional \[[1](#Codd-1970-CACM)\] para organizar dados como rela&ccedil;&otilde;es, apresentando-os de forma tabular como uma cole&ccedil;&atilde;o de tabelas em que cada uma delas consiste em um conjunto de linhas e colunas. Al&eacute;m disso, prov&ecirc;em operadores relacionais para manipula&ccedil;&atilde;o dos dados tabulares. Formalmente, um sistema de banco de dados deve estar em conformidade com as [12 regras de Codd](https://computing.derby.ac.uk/c/codds-twelve-rules/) para ser considerado relacional, entretanto nenhuma implementa&ccedil;&atilde;o comercial est&aacute; em conformidade com todas as regras. Dessa forma, o termo sistemas de banco de dados relacionais refere-se a uma ampla classe de sistemas de banco de dados que organizam dados como tabelas provendo operadores para manipula-los.

Sistemas gerenciadores de banco de dados relacionais (SGBDRs) foram muito populares nas d&eacute;cadas de 80 e 90 e ainda s&atilde;o amplamente utilizados devido &agrave; sua robustez, confiabilidade e seguran&ccedil;a. Al&eacute;m disso, o modelo de dados relacional prov&ecirc; uma algebra simples que torna f&aacute;cil a compreens&atilde;o sobre como dados podem ser organizados visando armazenamento e recupera&ccedil;&atilde;o eficientes.

## Palestras

1. Introdu&ccedil;&atilde;o aos sistemas de banco de dados [ (slides: [pdf](/slides/sld01.pdf)) ]
1. Arquitetura de SGBDRs [ (slides: [pdf](/slides/sld02.pdf)) ]
1. Linguagem de consulta estruturada (SQL) [ (slides: [pdf](/slides/sld04.pdf)) ]
1. &Aacute;lgebra relacional [ (slides: [pdf](/slides/sld06.pdf)) ]
1. Modelagem de dados: modelo de Entidade-Relacionamento (ER) [ (slides: [pdf](/slides/sld07.pdf)) ]
1. Modelagem de dados: modelo de Entidade-Relacionamento Estendido (EER) [ (slides: [pdf](/slides/sld08.pdf)) ]
1. Modelagem de dados: modelo relacional [ (slides: [pdf](/slides/sld09.pdf)) ]
1. Armazenamento de dados [ (slides: [pdf](/slides/sld17.pdf)) ]
1. Indexa&ccedil;&atilde;o [ (slides: [pdf](/slides/sld18.pdf)) ]
1. Processamento e otimiza&ccedil;&atilde;o de consultas [ (slides: [pdf](/slides/sld19.pdf)) ]
1. Ajuste de banco de dados [ (slides: [pdf](/slides/sld20.pdf)) ]
1. Processamento de transa&ccedil;&atilde;o [ (slides: [pdf](/slides/sld21.pdf)) ]
1. Controle de concorr&ecirc;ncia [ (slides: [pdf](/slides/sld22.pdf)) ]
1. Recupera&ccedil;&atilde;o de banco de dados [ slides ]

* Todas as palestras em um &uacute;nico arquivo [ (slides: [pdf](/slides/all.pdf)) ]

## Material

### Videos

1. [Channel: Intro to Database Systems](https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi) por Carnegie Mellon University.

### Outros Recursos

1. [The ANSI Blog: The SQL Standard – ISO/IEC 9075:2016](https://blog.ansi.org/?p=158690)
1. [Relax: Relational algebra calculator](https://dbis-uibk.github.io/relax/).

## Informa&ccedil;&atilde;o Adicional

Grande parte dos t&oacute;picos e palestras se basearam em \[[2](#Elmasri-2016-BOOK)\]. Materiais e atividades foram inspirados no curso da Carnegie Mellon [Intro to Database Systems](https://15445.courses.cs.cmu.edu/fall2019/).

## Notas

Agradecimento ao suporte no desenvolvimento dos *slides* a [Adriane de Jesus Miranda Gomes](https://www.linkedin.com/in/adrianegomes/) e [Victor Theles da Silva Costa](https://www.linkedin.com/in/victor-theles-silva-costa/).

## Refer&ecirc;ncias

<a name="Codd-1970-CACM"></a>\[[1][1]\] Edgar Frank Codd. A relational model of data for large shared data banks. Communications of the ACM. 13(6):377–387. 1970.

<a name="Elmasri-2016-BOOK"></a>\[[2][2]\] Ramez Elmasri, Shamkant B. Navathe. Fundamentals of database systems. 7ed. Pearson, 1280 p., 2016.

[1]: https://doi.org/10.1145%2F362384.362685
[2]: https://www.pearson.com/us/higher-education/program/Elmasri-Fundamentals-of-Database-Systems-7th-Edition/PGM189052.html
