[Vers&atilde;o em Portugu&ecirc;s](/README.md)

# Database Systems
This is a set of lectures and material on database systems providing an introduction to the main methods and algorithms for data storage and retrieval, particularly those used in traditional database management systems.

## Introduction
Database systems refers to a set of related data and the way it is organized and accessed. Formally, they are composed by an organized collection of data (database), a logical structure for data determining in which manner it can be stored, organized and manipulated (data model), and a software that provides access to the database for users and applications (database management system) \[[2](#Elmasri-2016-BOOK)\].

Relational database systems use a relational data model \[[1](#Codd-1970-CACM)\] to organize data as relations, presenting them in a tabular form as a collection of tables with each table consisting of a set of rows and columns. In addition, they provide relational operators to manipulate tabular data. Formally, a database system should conform to the [Codd's 12 rules](https://computing.derby.ac.uk/c/codds-twelve-rules/) to be considered relational, however no commercial implementation conform to all of the rules. Therefore, the term relational database systems describes a broader class of database systems that organize data as tables and provide operators to manipulate them.

Relational database management systems (RDBMS) were very popular in the 80's and 90's and are still widely used today due to their robustness, reliability and security. Furthermore, the relational data model provides a simple algebra that makes it easy to understand how data can be organized for efficient storage and retrieval.

## Lectures

1. Introduction to database systems [ (slides: [pdf](slides/sld01.pdf)) ]
1. The architecture of RDBMS [ (slides: [pdf](slides/sld02.pdf)) ]
1. Structured Query Language (SQL) [ (slides: [pdf](slides/sld04.pdf)) ]
1. Relational algebra [ (slides: [pdf](slides/sld06.pdf)) ]
1. Data modeling: Entity-Relationship model (ER) [ (slides: [pdf](slides/sld07.pdf)) ]
1. Data modeling: Extended Entity-Relationship model (EER) [ (slides: [pdf](slides/sld08.pdf)) ]
1. Data modeling: relational model [ (slides: [pdf](slides/sld09.pdf)) ]
1. Data storage [ (slides: [pdf](slides/sld17.pdf)) ]
1. Indexing [ (slides: [pdf](slides/sld18.pdf)) ]
1. Query processing and optimization [ (slides: [pdf](slides/sld19.pdf)) ]
1. Database tuning [ (slides: [pdf](slides/sld20.pdf)) ]
1. Transaction processing [ (slides: [pdf](slides/sld21.pdf)) ]
1. Concurrency control [ (slides: [pdf](slides/sld22.pdf)) ]
1. Database recovery [ slides ]

* All the lectures in one single file [ (slides: [pdf](slides/all.pdf)) ]

## Material

### Videos

1. [Channel: Intro to Database Systems](https://www.youtube.com/playlist?list=PLSE8ODhjZXjbohkNBWQs_otTrBTrjyohi) by Carnegie Mellon University.

### Other Resources

1. [The ANSI Blog: The SQL Standard – ISO/IEC 9075:2016](https://blog.ansi.org/?p=158690)
1. [Relax: Relational algebra calculator](https://dbis-uibk.github.io/relax/).

## Further Information

Most of the topics of the lectures are taken from \[[2](#Elmasri-2016-BOOK)\]. Material and assignments are mostly inspired by the Carnegie Mellon course [Intro to Database Systems](https://15445.courses.cs.cmu.edu/fall2019/).

## Acknowledgements

We are thankful for the support in the development of the slides given by [Adriane de Jesus Miranda Gomes](https://www.linkedin.com/in/adrianegomes/) and [Victor Theles da Silva Costa](https://www.linkedin.com/in/victor-theles-silva-costa/).

## References

<a name="Codd-1970-CACM"></a>\[[1][1]\] Edgar Frank Codd. A relational model of data for large shared data banks. Communications of the ACM. 13(6):377–387. 1970.

<a name="Elmasri-2016-BOOK"></a>\[[2][2]\] Ramez Elmasri, Shamkant B. Navathe. Fundamentals of database systems. 7ed. Pearson, 1280 p., 2016.

[1]: https://doi.org/10.1145%2F362384.362685
[2]: https://www.pearson.com/us/higher-education/program/Elmasri-Fundamentals-of-Database-Systems-7th-Edition/PGM189052.html
