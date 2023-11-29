# Entidades, relacionamentos e atributos

## Práticas eficazes

* Definição clara das regras de negócio: todas as regras de negócio precisam ser documentadas e entendidas. Dessa forma, será possível atender às necessidades do negócio.

* Comunicação aberta: discuta as decisões e troque ideias com a equipe de modelagem para garantir que todos estão na mesma página.

* Validação com os stakeholders: podem oferecer feedback sobre a precisão do modelo e se atende as necessidades de negócio.

* Conhecimento multidisciplinar: pessoas com diferentes perspectivas pode enriquecer o processo de abstração e tomar decisões mais abrangentes.

* Documentação detalhada: isso permite com que qualquer pessoa entenda as escolhas feitas, facilitando a colaboração e evitando ambiguidades.

* Iteração e melhoria contínua: à medida que o projeto avança, surge a necessidade de ajustes e refinamentos no modelo.

## Conceitos

**Abstração** é um processo mental que permite escolher / recortar um determinado aspecto de algo complexo para algo simples.

**Atributo simples:** é um tipo de atributo indivisível, ou seja, é um atributo atômico.

**Atributo composto:** pode ser dividido em partes menores que representam outros atributos, como endereço.

**Atributo multivalorado:** é aquele que pode ter um ou N (vários) valores associados a ele. Por exemplo: o atributo telefone de um cliente. Este pode ter um ou vários telefones.

**Atributo derivado e armazenado:** atributos derivados dependem de outro atributo ou até mesmo outra entidade para existir, como, idade e data de nascimento. Para descobrirmos a idade de uma pessoa, precisamos da sua data de nascimento. Então, consideramos o atributo idade como derivado do atributo data de nascimento, chamado, por sua vez, de atributo armazenado.

**Atributo chave:** é utilizado para identificar de forma única uma entidade, ou seja, os valores associados a esse atributo são distintos entre o conjunto de entidades.

**Alto nível:** modelagem de dados conceitual próxima da linguagem do ser humano.

**Baixo nível:** modelagem ligada à linguagem das máquinas.

**Cardinalidade:** sinônimo de conectividade e relacionamento entre entidades.

* (1,1) um-para-um
* (1,N) um-para-muitos
* (N,1) muitos-para-um
* (N,M) muitos-para-muitos

**Cardinalidade máxima:** número máximo de vezes que uma entidade X pode ocorrer em Y. Pode assumir o valor de 1 ou N (inúmeras vezes).

**Cardinalidade mínima (restrição de participação ou dependência de existência):** número mínimo de vezes que uma entidade X pode ocorrer em Y. Pode assumir o valor de 0 ou 1.

* **restrição total** ocorre quando todas as instâncias de uma entidade X precisam estar obrigatoriamente relacionadas a alguma instância da entidade Y.

* **restrição parcial** ocorre quando todas as instâncias de uma entidade X não precisam estar obrigatoriamente relacionadas a alguma instância da entidade Y.

**Chave primária:** atributos exclusivos de uma entidade.

1. Nunca se repete;
2. Não pode ser nulo;
3. Apenas entidades fortes possuem chave primária;

**Computer-Aided Software Engineering (CASE) ou Engenharia de Software Assistida por Computador** é uma ferramenta que utiliza diversas formas geométricas para desenvolver uma boa representação visual, a integração entre o diagrama entidade/relacionamento e o dicionário de dados, além de possibilitar uma mínima interação com o(a) usuário(a).

**Diagrama de Entidade e Relacionamento (DER)** é a representação gráfica do MER.

**Entidade** é um objeto único no mundo real. Pode ser abstrata (p. ex., departamento) ou concreta (p. ex. produto).

* **Forte:** possui sua própria chave primária e não depende de nenhuma outra entidade para ser identificada de forma única.
* **Fraca:** não possui uma chave primária única por si só e depende da relação com uma entidade forte para ser identificada.

**Modelo Entidade Relacionamento (MER)** é o modelo conceitual que descreve os objetos do mundo real e é o primeiro passo da modelagem de dados. Nele descrevemos as entidades, suas características (atributos) e como se relacionam.

**Mini-mundo** é um recorte do mundo real no formato de banco de dados.

**Modelo conceitual** é um esquema / desenho que demonstra as representações e conexões dos dados que serão armazenados.

**Modelo físico** é criado para descrever as tabelas, suas colunas e os relacionamentos. Diferente do modelo lógico, podemos utilizar uma linguagem padrão para realizar essa representação: a linguagem SQL, utilizada para trabalhar com banco de dados relacionais.

**Modelo lógico** é criado para realizar a descrição de como os dados serão armazenados no sistema. Ele explora os conceitos de domínio. Nesse modelo, descrevemos as entidades, os atributos, as chaves primárias e estrangeiras e os seus relacionamentos.

**Sistema Gerencial de Banco de Dados (SGBD)** é quem gerencia o banco de dados: inclui, altera e realiza consultas através de uma interface.
