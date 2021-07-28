# NoSQL: Tipos

Nesta seção são apresentados alguns casos de uso de problemas de armazenamento de dados associando-os a cada um dos tipos de bancos de dados NoSQL existentes mais apropriados para solução do problema.

## Chave-Valor

Casos típicos adequados para a utilização de bancos de dados NoSQL do tipo chave-valor são aqueles em que desejamos armazenar agregados simples de forma transitória. Exemplos desses casos são o armazenamento de dados de sessão de usuário, de perfis e preferências de usuário ou de carrinho de compras em *e-commerce*.

Geralmente, uma sessão de usuário na Web é exclusiva e recebe um valor exclusivo de *session-id*. Aplicações que armazenam *session-id* em disco ou em um banco de dados relacional se beneficiarão muito com a mudança para um armazenamento em banco de dados NoSQL do tipo chave-valor, uma vez que os dados sobre a sessão podem ser armazenados com uma única solicitação PUT ou recuperados com uma única solicitação GET. Esta operação de requisição única se torna muito eficiente, já que os dados sobre a sessão são armazenados em um único objeto.

Similarmente, usuários possuem um *id* e *nome*, além de muitos outros atributos que representam seus perfis e preferências, como *linguagem*, *cor*, *localização geográfica*, *fuso horário* e *lista de produtos preferidos*. Tais dados podem ser incorporados a um objeto, fazendo com que a obtenção das preferências de um usuário requeiram uma única operação GET. Não obstante, os *sites* de comércio eletrônico possuem carrinhos de compras vinculados ao usuário. Para que os carrinhos de compras estejam sempre disponíveis para o usuário durante sua sessão de navegação, seus dados de compra podem ser armazenados como valor associado à chave correspondente ao *id* do usuário.

Casos típicos de inadequação de um banco de dados NoSQL do tipo chave-valor são aqueles em que seja necessário manter relacionamento entre dados, ou em processamento de transações que requeiram restauração (*roll-back*) em caso de falhas, ou quando consultas a valores (e não chaves) sejam requeridas.

## Documento

Casos típicos adequados para a utilização de bancos de dados NoSQL orientados a documento são aqueles em que desejamos armazenar agregados complexos de forma permanente. Exemplos desses casos são o armazenamento de registros (*log*) de eventos, de páginas em plataforma de blog e gestão de conteúdo (CMS) e de catálogos de relatórios e produtos em sistemas analíticos e de *e-commerce*, por exemplo.





Casos típicos de inadequação de um banco de dados NoSQL orientados a documento são aqueles em que seja necessário o processamento de transações simultâneas em múltiplos documentos, ou quando consultas precisem varrer toda a estrutura dos agregados (documentos) para serem respondidas.

## Família de Colunas

## Grafo
