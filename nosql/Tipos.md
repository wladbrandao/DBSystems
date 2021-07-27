# NoSQL: Tipos

Nesta seção são apresentados os principais tipos de bancos de dados NoSQL, incluindo os bancos de dados orientados a documentos (**document store**), chave-valor (**key-value store**), orientados a colunas (**wide column store**) e os baseados em grafos (**graph store**).

<p align="center">
<img width="700" vspace="20" src="images/NoSQLTypes.png">
</p>

## Chave-Valor (*Key-Value*)

Bancos de dados chave-valor são geralmente implementados usando tabelas hash e são muito eficientes quando o acesso aos dados (valores) são efetuados exclusivamente por uma chave (primária). Os valores associados a cada chave podem assumir qualquer valor blob (*binary object*). No exemplo abaixo, o valor associado à chave de *id: 23811445* contém uma coleção de caracteres (*hello*), números (*213* e *0.15*) e um objeto binário.

Alguns dos bancos de dados NoSQL do tipo chave-valor mais populares atualmente são [BerkeleyDB](http://www.oracle.com/us/products/database/berkeley-db), [DynamoDB](http://aws.amazon.com/dynamodb), [HamsterDB](http://hamsterdb.com/), [MemcachedDB](http://memcached.org/), [Redis](http://redis.io/), [Riak](http://wiki.basho.com/Riak.html), e [Voldemort](http://project-voldemort.com/), uma versão de código aberto do DynamoDB.

<p align="center">
<img width="500" vspace="20" src="images/KeyValue.png">
</p>

## Documento (*Document*)

Este tipo de banco de dados armazena e recupera documentos de diferentes formatos, tais como XML, JSON, BSON, dentre outros. Esses documentos são organizados em uma estrutura hierárquica em árvore, podendo armazenar dados como mapas, coleções e valores escalares. Os documentos armazenados são geralmente semelhantes entre si, mas não necessariamente precisam ser iguais. No exemplo abaixo, o documento *Document 3* armazena os valores escalares *id*, *isActive* e *dob* e o valor *fullName* composto dos valores escalares *first* e *last*. Alguns dos bancos de dados NoSQL do tipo documento mais populares são [CouchDB](http://couchdb.apache.org/), [MongoDB](http://www.mongodb.org/), [OrientDB](http://www.orientdb.org/), [RavenDB](http://ravendb.net/) e [Terrastore](http://code.google.com/p/terrastore).

<p align="center">
<img width="500" vspace="20" src="images/Document.png">
</p>

## Coluna (*Wide-Column* / *Column-Family*)

Bancos de dados de famílias de colunas armazenam dados em famílias de colunas como linhas que possuem muitas colunas associadas com uma chave de linha. Famílias de colunas são grupos de dados relacionados que são frequentemente acessados conjuntamente. No exemplo apresentado abaixo o valor de chave **101** está associado a uma família de colunas **email**, **name** e **tel**, enquanto o valor de chave **103** está associado a uma família de colunas **email**, **name**, **tel** e **tel2**.
Alguns dos bancos de dados NoSQL do tipo documento mais populares são [Cassandra](http://cassandra.apache.org/), [DynamoDB](http://aws.amazon.com/dynamodb), [HBase](http://hbase.apache.org/) e [Hypertable](http://hypertable.org/).

<p align="center">
<img width="500" vspace="20" src="images/ColumnFamily.png">
</p>

## Grafo (*Graph*)

Bancos de dados orientados a grafos permitem armazenar entidades (nós) e relacionamentos (arestas) entre essas entidades, bem como suas propriedades. Arestas podem ser direcionais e tipificadas. No exemplo abaixo, os nós 1 e 2 possuem as propriedades *name* e *age* e estão relacionadas pela aresta *knows* com propriedade *weight* de valor *0.5*. A direção da aresta representa que o nó 1 *conhece* o nó 2, mas o nó 2 não *conhece* o nó 1.
Alguns dos bancos de dados orientados a grafos mais populares são [FlockDB](https://github.com/twitter/flockdb/), [Infinite Graph](http://www.infinitegraph.com/), [Neo4J](http://neo4j.org/) e [OrientDB](http://www.orientdb.org/).

<p align="center">
<img width="500" vspace="20" src="images/Graph.jpg">
</p>

## Refer&ecirc;ncias

<a name="Sadalage-2013-BOOK"></a>\[[1][1]\] Pramod J. Sadalage, Martin Fowler. NoSQL Distilled: A Brief Guide to the Emerging World of Polyglot Persistence. 1ed. Pearson, 2013.

[1]: https://doi.org/10.5555/2381014
