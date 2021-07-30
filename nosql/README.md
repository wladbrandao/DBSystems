# Sistemas de Banco de Dados NoSQL

Por d&eacute;cadas os sistemas de bancos de dados relacionais v&ecirc;m sendo a tecnologia preferencial para armazenamento e manipula&ccedil;&atilde;o de cole&ccedil;&otilde;es de dados, provendo persist&ecirc;ncia, controle de redund&ecirc;ncia e de concorr&ecirc;ncia e mecanismos de integra&ccedil;&atilde;ao de dados. Recentemente houve uma crescente demanda por processamento de volumes massivos de dados (*Big Data*) com baixa imped&acirc;ncia, caracter&iacute;sticas n&atilde;o suportadas pelos sistemas gerenciadores de bancos de dados relacionais vigentes.

Sistemas de banco de dados NoSQL prov&ecirc;m flexibilidade e alto desempenho no processamento de volumes massivos de dados ao abdicarem de r&iacute;gidas restri&ccedil;&otilde;es impostas pelo modelo de dados relacional, sendo capazes de realizar opera&ccedil;&otilde;es de forma distribu&iacute;da em *clusters* utilizando diferentes esquemas de dados \[[1](#Sadalage-2013-BOOK)\]. Al&eacute;m disso, h&aacute; um movimento crescente nas comunidades de desenvolvimento de software por distribui&ccedil;&atilde;o de dados via encapsulamento de bancos de dados e aplica&ccedil;&otilde;es para prover servi&ccedil;os em nuvem, em detrimento ao uso de sistemas gerenciadores de banco de dados como pontos centrais de integra&ccedil;&atilde;o.

## Tópicos

1. [Conceitos Básicos](docs/terminology.md)
1. [Aspectos Históricos](docs/history.md)
1. [Características](docs/properties.md)
1. [Benefícios](docs/benefits.md)
1. [Tipos](docs/types.md)
1. [Casos de Uso](docs/cases.md)
1. [Arquiteturas de Distribuição](docs/architecture.md)
1. [Modelo Tabular (Relacional)](docs/tabular.md)
1. [Modelo Chave-Valor](docs/keyvalue.md)
1. [Modelo Orientado a Coluna](docs/column.md)
1. [Modelo Orientado a Documento](docs/document.md)
1. [Modelo Orientado a Grafo](docs/graph.md)
1. [Apache Cassandra: NoSQL orientado a coluna](docs/cassandra.md)
1. [MongoDB: NoSQL orientado a documento](docs/mongo.md)
1. [Neo4J: NoSQL orientado a grafo](docs/neo4j.md)
1. [Redis: NoSQL chave-valor](docs/redis.md)

## Material

### Videos

1. [Introduction to MySQL](https://youtu.be/qI_g07C_Q5I) by Martin Fowler
1. [How do NoSQL databases work?](https://youtu.be/0buKQHokLK8)

### Outros Recursos

1. [What is NoSQL?](https://aws.amazon.com/nosql/)
1. [NoSQL Databases List by Hosting Data (2021)](https://hostingdata.co.uk/nosql-database/)
1. [Deep dive into NoSQL: A complete list of NoSQL databases (2014)](https://bigdata-madesimple.com/a-deep-dive-into-nosql-a-complete-list-of-nosql-databases/)
1. [How to Choose the Right NoSQL Database for Your Application? (2018)](https://www.dataversity.net/choose-right-nosql-database-application/)

## Refer&ecirc;ncias

<a name="Sadalage-2013-BOOK"></a>\[[1][1]\] Pramod J. Sadalage, Martin Fowler. NoSQL Distilled: A Brief Guide to the Emerging World of Polyglot Persistence. 1ed. Pearson, 2013.

[1]: https://doi.org/10.5555/2381014
