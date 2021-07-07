# Sistemas de Banco de Dados Relacionais

Sistemas de banco de dados referem-se ao conjunto de dados relacionados e sua respectiva forma de acesso e organiza&ccedil;&atilde;o. Formalmente, eles s&atilde;o compostos por uma cole&ccedil;&atilde;o de dados organizados (banco de dados), uma estrutura l&oacute;gica dos dados determinando a forma como podem ser armazenados, organizados e manipulados (modelo de dados), e um software que prov&ecirc; acesso ao banco de dados a usu&aacute;rios e aplica&ccedil;&otilde;es (sistema gerenciador de banco de dados) \[[2](#Elmasri-2016-BOOK)\].

Sistemas de banco de dados relacionais utilizam um modelo de dados relacional \[[1](#Codd-1970-CACM)\] para organizar dados como rela&ccedil;&otilde;es, apresentando-os de forma tabular como uma cole&ccedil;&atilde;o de tabelas em que cada uma delas consiste em um conjunto de linhas e colunas. Al&eacute;m disso, prov&ecirc;em operadores relacionais para manipula&ccedil;&atilde;o dos dados tabulares. Formalmente, um sistema de banco de dados deve estar em conformidade com as [12 regras de Codd](https://computing.derby.ac.uk/c/codds-twelve-rules/) para ser considerado relacional, entretanto nenhuma implementa&ccedil;&atilde;o comercial est&aacute; em conformidade com todas as regras. Dessa forma, o termo sistemas de banco de dados relacionais refere-se a uma ampla classe de sistemas de banco de dados que organizam dados como tabelas provendo operadores para manipula-los.

Sistemas gerenciadores de banco de dados relacionais (SGBDRs) foram muito populares nas d&eacute;cadas de 80 e 90 e ainda s&atilde;o amplamente utilizados devido &agrave; sua robustez, confiabilidade e seguran&ccedil;a. Al&eacute;m disso, o modelo de dados relacional prov&ecirc; uma algebra simples que torna f&aacute;cil a compreens&atilde;o sobre como dados podem ser organizados visando armazenamento e recupera&ccedil;&atilde;o eficientes.

## Palestras

1. Introdu&ccedil;&atilde;o \[ \( slides: [pdf](/relational/slides/sld01.pdf) \) | \( videos: [aula](https://youtu.be/vmElmxU1Ha0) \) \]
1. Modelos de Dados \[ \( slides: [pdf](/relational/slides/sld02.pdf) \) | \( videos: [aula](https://youtu.be/O1N7XbyOXzE) \) \]
1. Esquemas e Linguagens \[ \( slides: [pdf](/relational/slides/sld03.pdf) \) | \( videos: [aula](https://youtu.be/MdO4B7RMHYg) \) \]
1. Modelo Entidade-Relacionamento (ER) \[ \( slides: [pdf](/relational/slides/sld04.pdf) \) | \( videos: [aula](https://youtu.be/_y31cFi_ByY) \) \]
1. Modelo ER Estendido (EER) \[ \( slides: [pdf](/relational/slides/sld05.pdf) \) | \( videos: [aula](https://youtu.be/JFw0D8zZBVs) \) \]
1. Modelo Relacional \[ \( slides: [pdf](/relational/slides/sld06.pdf) \) | \( videos: [aula](https://youtu.be/yGH2k3PGMUw) \) \]
1. &Aacute;lgebra Relacional: B&aacute;sico \[ \( slides: [pdf](/relational/slides/sld07.pdf) \) | \( videos: [aula](https://youtu.be/ldv6-lUa3DU) \) \]
1. &Aacute;lgebra Relacional: Estendido \[ \( slides: [pdf](/relational/slides/sld08.pdf) \) | \( videos: [aula](https://youtu.be/h9tp7yjHwJU) \) \]
1. SQL: Defini&ccedil;&atilde;o de Dados \[ \( slides: [pdf](/relational/slides/sld09.pdf) \) | \( videos: [aula](https://youtu.be/5zwxgDf84j8) \) \]
1. SQL: Manipula&ccedil;&atilde;o de Dados \[ \( slides: [pdf](/relational/slides/sld10.pdf) \) | \( videos: [aula](https://youtu.be/XcxkF15Lc74) \) \]
1. Armazenamento em Mem&oacute;ria \[ \( slides: [pdf](/relational/slides/sld11.pdf) \) | \( videos: [aula](https://youtu.be/ngtawusmfBg) \) \]
1. Organiza&ccedil;&atilde;o de Dados em Mem&oacute;ria \[ \( slides: [pdf](/relational/slides/sld12.pdf) \) | \( videos: [aula](https://youtu.be/_rcM2m_5TuA) \) \]
1. Tecnologias de Armazenamento \[ \( slides: [pdf](/relational/slides/sld13.pdf) \) | \( videos: [aula](https://youtu.be/QO09bUKU1fM) \) \]
1. Indexa&ccedil;&atilde;o de Arquivo: N&iacute;vel &Uacute;nico \[ \( slides: [pdf](/relational/slides/sld14.pdf) \) | \( videos: [aula](https://youtu.be/cKU8zNz3jII) \) \]
1. Indexa&ccedil;&atilde;o de Arquivo: Multin&iacute;vel \[ \( slides: [pdf](/relational/slides/sld15.pdf) \) | \( videos: [aula](https://youtu.be/dsCIdOKROnk) \) \]
1. Processamento de Consulta \[ \( slides: [pdf](/relational/slides/sld16.pdf) \) | \( videos: [aula](https://youtu.be/8A7tWnoqyQo) \) \]
1. Otimiza&ccedil;&atilde;o de Consulta \[ \( slides: [pdf](/relational/slides/sld17.pdf) \) | \( videos: [aula](https://youtu.be/UX-COHcoJ8s) \) \]
1. Projeto F&iacute;sico \[ \( slides: [pdf](/relational/slides/sld18.pdf) \) | \( videos: [aula](https://youtu.be/x8Q0br-l3vo) \) \]
1. Processamento de Transa&ccedil;&atilde;o \[ \( slides: [pdf](/relational/slides/sld19.pdf) \) | \( videos: [aula](https://youtu.be/uBpB83R7usE) \) \]
1. Controle de Concorr&ecirc;ncia \[ \( slides: [pdf](/relational/slides/sld20.pdf) \) | \( videos: [aula](https://youtu.be/dScQNOxtiI8) \) \]

* Todas as palestras em um &uacute;nico arquivo \[ \( slides: [pdf](/relational/slides/all.pdf) \) \]

## Material

### Videos

1. [Sistemas de Banco de Dados](https://www.youtube.com/playlist?list=PLP034C8cuSalyokDrWr1PWm99RNZt5vuC) por Wladmir Cardoso Brand&atilde;o.
1. [Intro to Database Systems](https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi) por Carnegie Mellon University.

### Outros Recursos

1. [The ANSI Blog: The SQL Standard – ISO/IEC 9075:2016](https://blog.ansi.org/?p=158690)
1. [RelaX: Relational algebra calculator](https://dbis-uibk.github.io/relax/)
1. [Dummy Data for MYSQL Database](http://filldb.info/)

## Informa&ccedil;&atilde;o Adicional

Parte do conte&uacute;do das aulas se basearam em \[[2](#Elmasri-2016-BOOK)\]. Materiais e atividades foram inspirados no curso da Carnegie Mellon [Intro to Database Systems](https://15445.courses.cs.cmu.edu/fall2019/).

## Notas

Agradecimento ao suporte no desenvolvimento da vers&atilde;o 1.0 dos *slides* a [Adriane de Jesus Miranda Gomes](https://www.linkedin.com/in/adrianegomes/) e [Victor Theles da Silva Costa](https://www.linkedin.com/in/victor-theles-silva-costa/).

## Refer&ecirc;ncias

<a name="Codd-1970-CACM"></a>\[[1][1]\] Edgar Frank Codd. A relational model of data for large shared data banks. Communications of the ACM. 13(6):377–387. 1970.

<a name="Elmasri-2016-BOOK"></a>\[[2][2]\] Ramez Elmasri, Shamkant B. Navathe. Fundamentals of database systems. 7ed. Pearson, 2016.

<a name="Silberschatz-2016-BOOK"></a>\[[3][3]\] Avi Silberschatz, Henry F. Korth, S. Sudarshan. Database System Concepts. 6ed. McGraw-Hill, 2019.

<a name="Date-2004-BOOK"></a>\[[4][4]\] Christopher J. Date. An Introduction to Database Systems. 8ed. Pearson, 2004.

[1]: https://doi.org/10.1145%2F362384.362685
[2]: https://www.pearson.com/us/higher-education/program/Elmasri-Fundamentals-of-Database-Systems-7th-Edition/PGM189052.html
[3]: https://www.db-book.com/db7/
[4]: https://www.pearson.com/us/higher-education/program/Date-An-Introduction-to-Database-Systems-8th-Edition/PGM274345.html
