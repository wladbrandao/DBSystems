# NoSQL: Benefícios

Nesta seção são apresentados os principais benefícios de utilização dos bancos de dados NoSQL. Em grande parte tais benefícios advêm das características marcantes desses bancos de dados.


## Capacidade de Armazenamento

Bancos de dados relacionais são tipicamente implementados em uma arquitetura verticalmente escalável baseada no uso de computadores cada vez maiores, com mais CPUs e memória, para melhorar o desempenho. Diferentemente, bancos de dados NoSQL foram criados na era da computação em nuvem, o que tornou possível implementar mais facilmente uma arquitetura horizontalmente escalável, onde a escalabilidade é alcançada distribuindo o armazenamento de dados em um grande *cluster* computacional. Para aumentar a capacidade de armazenamento, mais computadores são adicionados ao *cluster*.

Essa arquitetura de expansão horizontal é particularmente fácil de ser implementada em ambientes de computação em nuvem, onde novos computadores e armazenamento podem ser facilmente adicionados a um *cluster*. Além disso, tal arquitetura de escalabilidade fornece um caminho claro para escalabilidade quando o volume de dados ou tráfego aumenta. Alcançar o mesmo tipo de escalabilidade com uma arquitetura vertical pode ser caro e requerer muita engenharia, tornando-se inviável.

## Desempenho de Processamento

A mesma arquitetura de expansão horizontal que garante grande capacidade de armazenamento também garante elevado desempenho de processamento. Múltiplos nós em *cluster* computacional são usados para processamento de dados tipicamente usando padrões de paralelismo e distribuição como o *map-reduce*, o que confere aos bancos de dados NoSQL alta capacidade de processamento paralelo e distribuído de dados. Acréscimos significativos na capacidade de processamento podem ser facilmente obtidos simplesmente adicionando mais computadores ao *cluster* computacional existente.


## Disponibilidade

Em uma arquitetura verticalmente escalável a disponibilidade do sistema está condicionada à disponibilidade do servidor de banco de dados. Já em uma arquitetura horizontal a disponibilidade depende da forma como os dados são distribuídos entre os nós do *cluster* computacional.

A fragmentação (*sharding*) e replicação (*replication*) de dados obtidos numa arquitetura baseada em *cluster* computacional garantem uma elevada disponibilidade de dados. Particularmente, um mesmo dado pode estar fragmentado entre diferentes nós computacionais tornando a recuperação mais eficiente, enquanto a mesma cópia de um dado pode se encontrar armazenada em diferentes nós computacionais, aumentando a disponibilidade do sistema. Dessa forma, enquanto um nó pode estar indisponível ou muito ocupado com o processamento de um grande volume de requisições, outros nós com uma cópia dos dados requisitados podem estar menos ocupados, aumentando assim a disponibilidade do sistema.

## Flexibilidade

Bancos de dados relacionais armazenam dados em tabelas estruturadas que possuem um esquema rígido predefinido. Para usar esse tipo de solução um modelo de dados relacional deve ser projetado antes mesmo dos dados serem transformados e carregados no banco de dados. Ao serem usados ​​em aplicações os dados devem ser recuperados usando SQL e sua estrutura deve ser adaptada à estrutura usada na aplicação. Da mesma forma, quando os dados são gravados de volta, eles devem ser transformados novamente na estrutura de tabelas relacionais.

Já os bancos de dados NoSQL têm se mostrado populares porque permitem que os dados sejam armazenados de maneiras mais flexível, ou seja, mais fáceis de se transformar ou mais próximos da forma como os dados são usados pelas aplicações. Sendo assim, menos transformações são necessárias quando os dados são armazenados ou recuperados para uso. Sejam os dados estruturados, não estruturados ou semiestruturados, eles podem ser armazenados e recuperados mais facilmente, o que torna o trabalho de um desenvolvedor de aplicações mais produtivo.

Além disso, os esquemas de muitos bancos de dados NoSQL são flexíveis e estão sob o controle dos desenvolvedores, facilitando a adaptação do banco de dados a novas formas de organização de dados. Isso remove gargalos no processo de desenvolvimento associados ao pedido de um administrador de banco de dados para reprojetar um banco de dados relacional.

## Tolerância a Falhas

A replicação (*replication*) de dados obtida numa arquitetura baseada em *cluster* computacional garante proteção contra falhas. Em uma arquitetura verticalmente escalável a capacidade de tolerância a falhas do sistema está condicionada à disponibilidade do servidor de banco de dados. Problemas no servidor acarretam falhas no sistema.
Já em uma arquitetura horizontal com replicação, a indisponibilidade de um nó computacional não acarreta falhas no sistema que pode continuar operando a partir das cópias replicadas em outros nós.


## Poliglotismo (*Polyglot Persistence*)

Problemas de natureza diferentes requerem soluções de armazenamento diferentes, e tentar usar uma única solução de banco de dados para todos os problemas tipicamente resulta em baixo desempenho. O armazenamento de dados transacionais, o *cache*
de sessões de usuário, percorrer caminhos em grafos para encontrar itens correlacionados a outros são
problemas essencialmente diferentes e a utilização de uma mesma solução de armazenamento não parece ser uma decisão inteligente. Mesmo os requisitos de um processamento transacional (OLTP) ou analítico (OLAP), que geralmente demandam bancos de dados relacionais, podem ser muito diferentes.

Aplicações complexas combinam diferentes tipos de problemas, sendo que um mesmo problema pode requerer diferentes mecanismos de armazenamento, cada um capaz de lidar com diferentes subproblemas. Dessa forma, escolher a solução de armazenamento correta para cada subproblema pode ser mais produtivo do que tentar encaixar todos os subproblemas em uma única solução de armazenamento.

Bancos de dados NoSQL oferecem uma miríade de soluções de armazenamento capazes de lidar com problemas de naturezas diferentes que demandem por exemplo o armazenamento de pares chave-valor, documentos ou grafos, o que enriquece as opções disponíveis para além da escolha de uma opção relacional única para toda sorte de problema.

# Refer&ecirc;ncias

<a name="Sadalage-2013-BOOK"></a>\[[1][1]\] Pramod J. Sadalage, Martin Fowler. NoSQL Distilled: A Brief Guide to the Emerging World of Polyglot Persistence. 1ed. Pearson, 2013.

[1]: https://doi.org/10.5555/2381014
