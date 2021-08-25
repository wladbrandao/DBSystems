# NoSQL: Casos de Uso

Nesta seção são apresentados alguns casos de uso de problemas de armazenamento de dados associando-os a cada um dos tipos de bancos de dados NoSQL existentes mais apropriados para solução do problema.

## Chave-Valor

Casos típicos adequados para a utilização de bancos de dados NoSQL do tipo chave-valor são aqueles em que desejamos armazenar agregados simples de forma transitória. Exemplos desses casos são o armazenamento de dados de sessão de usuário, de perfis e preferências de usuário ou de carrinho de compras em *e-commerce*.

Geralmente, uma sessão de usuário na Web é exclusiva e recebe um valor exclusivo de *session-id*. Aplicações que armazenam *session-id* em disco ou em um banco de dados relacional se beneficiarão muito com a mudança para um armazenamento em banco de dados NoSQL do tipo chave-valor, uma vez que os dados sobre a sessão podem ser armazenados com uma única solicitação PUT ou recuperados com uma única solicitação GET. Esta operação de requisição única se torna muito eficiente, já que os dados sobre a sessão são armazenados em um único objeto.

Similarmente, usuários possuem um *id* e *nome*, além de muitos outros atributos que representam seus perfis e preferências, como *linguagem*, *cor*, *localização geográfica*, *fuso horário* e *lista de produtos preferidos*. Tais dados podem ser incorporados a um objeto, fazendo com que a obtenção das preferências de um usuário requeiram uma única operação GET. Não obstante, os *sites* de comércio eletrônico possuem carrinhos de compras vinculados ao usuário. Para que os carrinhos de compras estejam sempre disponíveis para o usuário durante sua sessão de navegação, seus dados de compra podem ser armazenados como valor associado à chave correspondente ao *id* do usuário.

Casos típicos de inadequação de um banco de dados NoSQL do tipo chave-valor são aqueles em que seja necessário manter relacionamento entre dados, ou em processamento de transações que requeiram restauração (*roll-back*) em caso de falhas, ou quando consultas a valores (e não chaves) sejam requeridas.

## Documento

Casos típicos adequados para a utilização de bancos de dados NoSQL orientados a documento são aqueles em que desejamos armazenar agregados complexos de forma permanente. Exemplos desses casos são o armazenamento de registros (*log*) de eventos, de páginas em plataforma de blog e gestão de conteúdo (CMS) e de catálogos de relatórios e produtos em sistemas analíticos e de *e-commerce*, por exemplo.

Eventos, como estados ou erros de aplicações, apresentam dados heterogêneos que podem mudar com muita frequência. Dessa forma, um modelo de dados flexível como o orientado a documento se torna uma escolha efetiva para este tipo de aplicação. Da mesma forma, em plataformas de blog e de gestão de conteúdo, onde postagens e páginas HTML não têm esquemas de dados predefinidos, a adoção de modelos de dados flexíveis que propiciam o armazenamento de dados heterogêneos e mutáveis é apropriada.

Casos típicos de inadequação de um banco de dados NoSQL orientados a documento são aqueles em que seja necessário o processamento de transações simultâneas em múltiplos documentos, ou quando consultas precisem varrer toda a estrutura dos agregados (documentos) para serem respondidas.

## Família de Colunas

Casos típicos adequados para a utilização de bancos de dados NoSQL orientados a família de colunas são aqueles em que desejamos armazenar agregados complexos de forma permanente. Similarmente aos bancos de dados NoSQL orientados a documento, exemplos desses casos são o armazenamento de registros (*log*) de eventos, de páginas em plataforma de blog e gestão de conteúdo (CMS). Um caso particular de utilização é o armazenamento de contadores em sistemas analíticos ou mesmo para agregados complexos com data de expiração.

Eventos são frequentemente registrados para manutenção de histórico e raramente pesquisados. Nesses casos, um modelo de dados flexível que garanta gravação eficiente como o de família de colunas se torna a escolha ideal. Além disso, em plataformas de blog e de gestão de conteúdo, usando famílias de colunas é possível armazenar entradas de blog com tags, categorias, links e *trackbacks* em colunas diferentes. Os comentários podem ser armazenados na mesma linha ou movidos para um espaço de chaves (*keyspace*) diferente. Da mesma forma, usuários e postagens do blog podem ser colocados em diferentes famílias de colunas. Frequentemente, aplicativos Web precisam contar e categorizar os visitantes de uma página para realizar análises de uso e consumo de recursos, o que pode ser facilmente implementado por contadores armazenados em tipos especiais de colunas.

Casos típicos de inadequação de um banco de dados NoSQL orientados a família de colunas são aqueles em que seja necessário o processamento de transações conservando as propriedades ACID, ou mesmo quando o esquema para organização dos dados não esteja maduro o suficiente, uma vez que mudanças na organização dos dados podem acarretar reestruturações complexas na organização das famílias de colunas.

## Grafo

Casos típicos adequados para a utilização de bancos de dados NoSQL orientados a grafo são aqueles em que desejamos armazenar agregados complexos, em especial conexões complexas entre dados, de forma permanente. Exemplos desses casos são o são o armazenamento de redes complexas de objetos interconectados, serviços de roteamento e geo-referenciamento e sistemas de recomendação.

Redes sociais ou mesmo redes tecnológicas complexas, em que as relações entre os objetos frequentemente precisam ser acessadas e pesquisadas são casos típicos de utilização de bancos de dados NoSQL orientados a grafo. Situações de roteamento de objetos, em que nós devem ser visitados seguindo rotas de menor custo, ou mesmo sistemas geo-referenciados em que cada localidade (referência geográfica) pode ser mapeada como um nó, e o conjunto de nós podem ser modelados como um grafo para cálculo de distâncias entre nós por exemplo, também são casos típicos de utilização de bancos de dados NoSQL orientados a grafo.

Casos típicos de inadequação de um banco de dados NoSQL orientados a grafo são aqueles em que seja necessário a atualização periódica de um grande volume de dados, o que pode acarretar atualizações de propriedades de múltiplos nós e arestas do grafo, tornando tal operação muito ineficiente.

# Refer&ecirc;ncias

<a name="Sadalage-2013-BOOK"></a>\[[1][1]\] Pramod J. Sadalage, Martin Fowler. NoSQL Distilled: A Brief Guide to the Emerging World of Polyglot Persistence. 1ed. Pearson, 2013.

<a name="Fowler-2012-VIDEO"></a>\[[2][2]\] Martin Fowler. Introduction to NoSQL: When and why to use a NoSQL database, 2012.

[1]: https://doi.org/10.5555/2381014
[2]: https://www.youtube.com/watch?v=qI_g07C_Q5I&t=2680s
