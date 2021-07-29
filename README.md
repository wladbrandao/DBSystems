# Sistemas de Banco de Dados
Este &eacute; um conjunto de materiais sobre sistemas de banco de dados provendo uma introdu&ccedil;&atilde;o aos principais m&eacute;todos e algoritmos usados para armazenamento e recupera&ccedil;&atilde;o de dados. O conte&uacute;do se divide em dois t&oacute;picos: [sistemas de banco de dados relacionais](/relational) e [sistemas de banco de dados NoSQL](/nosql).

## Banco de Dados, Informação e Conhecimento

Existe uma confusão feita por muitas pessoas quanto aos conceitos de banco de dados, bases de informação e bases de conhecimento, em grande parte oriunda da imprecisão semântica na definição dos conceitos de **dado**, **informação** e **conhecimento**. Longe de buscar uma definição universal para tais conceitos, cabe aqui estabelecer uma definição que ajude a eliminar essa imprecisão semântica.

<p align="center">
<img width="700" vspace="20" src="nosql/images/Data2Wisdom.jpg">
</p>

Por **dado** entende-se um conjunto de códigos, símbolos ou sinais capazes de serem assimilados sensorialmente, sendo eles decifráveis ou não. Por exemplo, um conjunto de desenhos feitos em pedra por homens das cavernas podem não ser decifráveis, mas ainda assim correspondem a um conjunto de símbolos assimilados sensorialmente. Por **informação** entende-se uma ideia, um conceito com semântica bem definida. Por exemplo, a partir do momento em que um desenho (símbolo) é decifrado e associado a um objeto mental, temos uma ideia, uma informação. Já por **conhecimento** entende-se uma cadeia de correlações entre ideias. Por exemplo, a partir do momento em que associamos a ideia de trovão e nuvem podemos estabelecer uma correlação com a ideia de chuva.

Por mais que os conceitos de dado, informação e conhecimento estejam relacionados, cada um deles remete a um objeto diferente. Dessa forma, é também importante aqui diferenciarmos os conceitos de banco de dados, base de informação e base de conhecimento. Enquanto um **banco de dados** se ocupa do armazenamento e recuperação eficientes de símbolos, uma **base de informação** se ocupa do armazenamento e recuperação eficientes de outro tipo de objeto, as ideias, muitas vezes expressas em textos em linguagem natural. Já uma **base de conhecimento** se ocupa do armazenamento e recuperação eficientes de correlações, muitas vezes expressas em linguagens formais, como a lógica e a matemática ou mesmo incorporadas em processos.

## Sistemas de Banco de Dados

Sistemas de banco de dados referem-se ao conjunto de dados relacionados e sua respectiva forma de acesso e organiza&ccedil;&atilde;o, sendo compostos por uma cole&ccedil;&atilde;o de dados organizados (banco de dados), uma estrutura l&oacute;gica determinando a forma como os dados podem ser armazenados, organizados e manipulados (modelo de dados), e um software que prov&ecirc; acesso ao banco de dados a usu&aacute;rios e aplica&ccedil;&otilde;es (sistema gerenciador de banco de dados).

## Sistemas de Banco de Dados Relacionais

Sistemas de banco de dados relacionais referem-se aos sistemas compostos por bancos de dados que adotam um modelo de dados relacional para organizar dados de forma tabular como uma coleção de tabelas em que cada uma delas consiste em um conjunto de linhas e colunas, bem como pelo software gerenciador do banco de dados capaz de armazenar e processar dados relacionais de forma segura e eficiente. Nesses sistemas a descrição formal dos dados é fornecida previamente pelos metadados descritivos presentes no esquema de dados.

## Sistemas de Banco de Dados NoSQL

Sistemas de banco de dados NoSQL referem-se aos sistemas compostos por bancos de dados que não adotam um modelo de dados relacional para armazenamento persistente de volumes massivos de dados (*big data*), sendo muitas vezes utilizados para superar as barreiras de escalabilidade e impedância presentes nos sistemas de banco de dados relacionais. Muitos desses sistemas operam em *cluster* computacional e sem um esquema de dados predefinido.
