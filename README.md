# dio-imersao-spring-framework-com-springboot
Repositório com alguns projetos de exemplos utilizando o framework spring boot, onde foi ministrado desde o exemplo mais simples, até um exemplo de conexão com o banco de dados postgres.

# MAVEN

O Maven é uma ferramenta desenvolvida pela Apache, ela serve para gerenciar as dependências e automatizar seus builds.

Já o pom.xml é o arquivo de configuração do Maven.

# CRIANDO PROJETO COM MAVEN

mvn archetype:generate -DgroupId=one.digitalinnovation -DartifactId=quick-start-maven -Darchetype=maven-archetype-quickstart -DinteractiveMode=false

# COMPILAR CLASSES
mvn compiler
* Cria a pasta "target"

# Teste
mvn test
* Faz asserção das classes

# EMPACOTAR O SOFTWARE (CRIA O JAR DA APLICAÇÃO )
mvn package
* Cria em "target" um jar.

# LIMPAR A PASTA TARGE
mvn clean

# COMO ENCONTRAR DIFERENTES TIPOS DE PROJETO MAVEN
* Digitar na internet "maven archetype list"

# ENTENDO O POM
POM = Project Object Model
- unidade fundamental de trabalho
- formato XML
- detalha o projeto
- detalha como construir o projeto
- Maven sempre procura pelo pom.xml para realizar sua execução

# Mais detalhes pom.xml
- Nome do projeto
- dependências
- módluos
- configurações de build
- detalhes do projeto (nome, descrição, licença, url)
- configurações de ambiente (repositórios, tracking, profiles)
- exemplos

# OBS:
Existe também o SUPERPOM um elemento pai do pom

# REPOSITÓRIOS
Locais onde encontrar bibliotecas e plugins que o Maven provê
- tipos: local e remoto

## Remoto
- é o local central utilizado pelo Maven para buscar os artefatos.
- configurado automaticamente pelo Super POM para utilizar o Maven central

## Local
- é o repositório na máquina utilizado pelo Maven para buscar os artefatos

- estratégia de caching
- Localizações
- Windows: %USERPROFILE%\.m2\repository

# ORM
* Object-Relational Mapping, em português, mapeamento objeto-relacional, é um recurso para aproximar o paradigma da orientação a objetos ao contexto de banco de dados relacional.

* O uso de ORM é realizado através do mapeamento de objeto para uma tabela por uma biblioteca ou framework.

# PALAVRA CHAVES
* ORM = APROXIMAR PARADIGMA DA POO À BANCO DE DADOS RELACIONAL.

# JPA
JPA é uma especificação baseada em interfaces, que através de um framework realiza operações de persistência de objetos em Java.
Ex framework: Hibernate, eclipseLink, oracleTopLink, openJpa

# MAPEAMENTO
Aspectos das anotações de mapesamento JPA:

* Identificação
* Definição
* Relacionamento
* Herança
* Persistência


# SPRING DATA JPA
* Adiciona uma camada sobre o JPA, isso significa que ele usa todos os recursos definidos pela especificação JPA, especialmene os mapeamentos de entidade e os recursos de persistência baseado em interfaces e anotações. Por isso, o Spring Data JPA adiciona seus próprios recursos, como uma implementação sem código do padrão de repositório e a criação de consultas de banco de dados a partir de nomes de métodos

* O projeto Spring Data Jpa facilita a implementantação do padrão Repository através de AOP (Aspect Oriented Programming - Programçaõ Orientada a aspectos). - COMO FORMA DE SUBSTITUIR O DAO.

