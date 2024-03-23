# Java AI Powered
- Curso da DIO sobre desenvolvimento com Java

## Ganhando produtividade em Java com Spring Framework

### Bootcamps DIO: educação Gratuita e Empregabilidade Juntas!
- Já foi concluído no curso de desenvolvimento de jogos

### Contextualizando o Desenvolvimento Web com Spring Boot 3
- Visão Geral
  - Intellij
  - JDK 17+
  - Kotlin 1.7.22
  - Sintaxe básica Kotlin
  - Conhecimento acerca de POO
- Entendendo a arquitetura REST — Parte 1
  - API (Application Programming Interface)
  - Funciona em termos de cliente e servidor
  - API SOAP usam XML
    - Menos flexivel e mais popular antigamente
  - API RPC
    - O cliente conclui uma função (ou um procedimento) no servidor e o servidor envia a saída de volta ao cliente
  - API Websocket
    - O servidor pode enviar mensagens de retorno de chamada a clientes conectados, tornando-os mais eficientes que a API REST
  - API REST
    - O cliente envia solicitações ao servidor como dados
    - O servidor usa essa entrada do cliente para iniciar funções internas e retorna os dados de saída ao cliente
  - O que são API REST?
    - REST significa transferência representacional de estado
    - Clientes e servidores trocam dados usando HTTP
    - O HTTP permite criar, atualizar, pesquisar, executar e remover operações, atuando sob determinados recursos
    - A principal característica da API REST é a ausência de estado
    - http://localhost:1234/hrservices/v1/users/{id}
      - http é o protocolo
      - localhost é o host
      - `1234` é a porta
      - hrservices é o application context
      - v1 é a versão
      - users é o resource
      - `{id}` é o parametro
- Entendendo a arquitetura REST — Parte 2
  - Explicação sobre métodos HTTP e retornos
  - JSON
    - É um formato de troca de dados entre sistemas independentes de linguagem de programação derrivado do javascript
    - É frequentemente utilizado em aplicações Ajax, configurações, banco de dados e (serviços) ‘web’ RESTful
- Overview do Spring Framework
  - Objetivo de facilitar desenvolvimento de aplicações
  - Baseado na IoC (Inversão de Controle) e DI (Injeção de dependência) utilizando beans
  - Spring Boot é utilizado para trazer agilidade com as configurações iniciais
  - Spring Framework tem 20 modulos
  - Spring Boot
    - Abstrair e facilitar a configuração de, por exemplo:
      - Servidores
      - Gestão de dependências
      - Configuração de bibliotecas
      - Métricas e health checks
    - Spring Boot Starters
      - Dependências que agrupam outras dependências com um propósito em comum
      - Exemplo:
        - spring-boot-starter-test
    - Spring Initializr
      - É uma UI que permite a criação de projetos Spring Boot de forma facilitada
- Arquitetura de três camadas com Spring Boot
  - Separa em lógica de apresentação, lógica de negócio e lógica de acesso a dados
  - Torna o sistema mais flexível
  - Arquitetura Projeto Spring
    - Postman Client
      - JSON e DTO
    - Controller
      - API Layer
    - Service
      - Business Logic
    - DAO (repository)
      - Persistence logic
    - DB
  - Arquivo de configuração
    - Ao trabalhar com Spring Boot, nos deparamos com várias configurações que devem ser realizadas
    - O Spring Boot permite utilizar 2 diferentes arquivos de configurações:
      - application.properties
      - application.yml

### Versionamento de código com Git e Github
- Já foi concluído no curso de desenvolvimento de jogos

### Desafios de Projetos: Crie um `Portfólio` Vencedor
- Apresentação
  - É visto por todos da DIO
- PBL, `Portfólio`, Competências e Empregabilidade
  - Aprendizado Baseado em Projetos
  - Bom para demonstrar conhecimentos técnicos
  - É bom para ganhar conhecimento, mas não ajuda a conseguir uma vaga no mercado de trabalho
  - Tenha empatia com pessoas que estudam programação
- A importância dos desafios de projeto, na prática
  - Mostrou o módulo contribuindo num projeto `open source` no github
  - As aulas de construção são melhores que os desafios
  - Todos os projetos são entregues no github
  - README é o arquivo onde fica tudo sobre o projeto
  - Para contribuir para um desafio deve fazer um `fork`
  - É possível ver os projetos no perfil da DIO

### Contribuindo num Projeto Open Source no Github
- Já foi concluído no curso de desenvolvimento de jogos

### Imersão no Spring Framework com Spring Boot

#### Apresentação Inicial
- Abertura
  - Explicação bem rápida sobre o curso
  - Gleyson Sampaio
- Visão geral do curso
  - Imersão no Spring Framework
  - Dez anos de experiência
  - Spring Versus JavaEE
  - O que é Spring Boot?
  - Conceito de IoC / DI
  - Beans \ Autowired \ Scopes
  - Spring Data JPA
- Spring Framework
  - Fundamentos
  - Certificado Java SE 6 Programmer
  - O que é Spring Framework?
    - `Framework Open Source` desenvolvido para a plataforma Java baseado nos padrões de projetos
      - Inversão de Controle
      - Injeção de dependência
    - A sua estrutura é composta por módulos
      - Tem o objetivo de reduzir a complexidade no desenvolvimento de aplicações simples ou corporativas
    - Módulos
      - Data Access / Integration
        - JDBC
        - ORM
        - OXM
        - JMS
        - Transactions
      - Web (MVC / Remoting)
        - Web
        - Servlet
        - Portlet
        - Struts
      - AOP
      - Aspects
      - Instrumentation
      - Core Container
        - Beans
        - Core
        - Context
        - Expression Language
      - Test
  - Spring Versus JavaEE
    - JavaEE tem muita burocracia
    - Spring foi um movimento para simplificar o desenvolvimento
  - Conceito de IoC / DI
    - Inversão de Controle ou IoC (Inversion of Control)
      - Trata-se do redirecionamento do fluxo de execução de um código retirando parcialmente o controle sobre ele e delegando-o para um container
      - O principal propósito é minimizar o acoplamento do código
      - Sem o IoC era necessário criar o objeto e depois utilizá-lo
      - Com o IoC o container cria os objetos necessários
    - Injeção de dependências
      - É um padrão de desenvolvimento com a finalidade de manter baixo o nível de acoplamento entre módulos de um sistema
      - O container tem os objetos reais, mas as implementações são feitas via ‘interface’ por injeção de dependência
  - Beans \ Autowired \ Scopes
    - Beans
      - Objeto instanciado (criado), montado e gerenciado por um container através do princípio da inversão de controle
    - Scopes
      - Singleton
        - O container do Spring IoC define apenas uma instância do objeto
      - Prototype
        - Será criado um objeto a cada solicitação ao container
      - Spring Beans Scopes
      - HTTP
        - Request
          - Um bean será criado para cada requisição HTTP
          - Os objetos existirão enquanto a requisição estiver em execução
        - Session
          - Um bean será criado para a sessão de utilizador
          - Precisamos acessar a mesma solicitação duas vezes para testar os escopos específicos da ‘web’
        - Global
          - `Application scope` cria um bean para o ciclo de vida do contexto da aplicação
          - Objetos compartilhados por toda a aplicação
    - Autowired
      - Uma anotação (indicação) onde deverá ocorrer uma injeção automática de dependência
      - `byName`: buscado um método set que corresponde ao nome do Bean
      - `byType`: considerado o tipo da classe para inclusão do Bean
      - `byConstructor`: usamos o construtor para incluir a dependência

#### Projeto Spring Boot
- Conhecendo o Spring Boot
  - O que é Spring Boot?
    - Enquanto o Spring Framework é baseado no padrão de injeção de dependências
    - O Spring Boot foca na configuração automática
    - Antes do Spring Boot
      - Dependência individual
      - Verbosidade
      - Incompatibilidade de versões
      - Complexidade de gestão
      - Configurações complexas e repetitivas
  - Configurações manuais
    - Antes do Spring todas as configurações eram feitas manualmente
    - O Spring Boot veio para não precisar mais fazer esse processo manualmente
  - Starters
    - São descritores de dependências
    - São pacotes de dependências com todas as dependências necessárias para realizar uma ação
    - Coesão
    - Versões compatíveis
    - Otimização de tempo
    - Configurações simples
    - Foco no negócio
  - Principais starters
    - data-jpa: Integração com o banco de dados via JPA — Hibernate
    - data-mongodb: Integração com banco de dados MongoDB
    - `web`: Inclusão do container Tomcat para aplicações REST
    - web-services: WebServices baseados na arquitetura SOAP
    - batch: Implementação de `JOBs` de processos
    - `test`: Disponibilização de recursos para testes unitários como JUnit
    - openfeign: Client HTTP baseado em interfaces
    - actuator: Gestão de monitoramento da aplicação
  - Configuração de fábrica
- Primeiros passos
  - Criando um projeto com o Initializr
    - https://start.spring.io/
  - Importando o projeto maven no Intellij
    - Descompactar o projeto gerado no Initializr
    - Abrir no Intellij
  - Conhecendo a estrutura spring boot
    - src/main
      - pasta raiz dos projetos java
      - java
        - Dentro desse pacote que fica o código java
        - Existe a classe principal que inicia o spring boot
    - pom.xml
      - A propria aplicação tem um conceito de spring boot
    - test
      - Já tem uma classe de teste da aplicação
    - application.properties
      - Todas as configurações da aplicação serão feitas nesse arquivo
  - Bean e CommandLineRunner
    - Para dizer que uma classe é um Bean que será gerenciado pelo Spring deve utilizar a anotação @Component
    - O CommandLineRunner é utilizado, pois, não utilizamos o pacote, `web` do spring boot
- Beans versus Components
  - Quando usar @Bean
    - Utilizado quando não tem acesso ao código-fonte
    - Exemplo é o CommandLineRunner
  - Quando usar @Component
    - Serão componentes scaneados pela aplicação
    - Utiliza @Component quando tem acesso ao código-fonte
    - Evita dar o comando `new` para utilizar os métodos da classe
  - Implementar a IoC e DI
- Scopes - Singleton ou Prototype
  - Conceito de Scope
  - Configurando objeto Singleton
    - Apenas uma instância na aplicação
  - Configurando objetos Prototype
    - Pode ter vários de acordo com necessidade da aplicação
- Properties value
  - O poderoso application.properties
    - Pode ser colocado o valor dentro do application.properties
  - @Value
    - Com o @Value pegar o valor que foi definido no application.properties
  - Default Value
- Configuration properties
  - O poderoso application.properties
  - @ConfigurationProperties(prefix)
    - Deixa centralizado numa classe as propriedades
- Conceito de ORM e JPA
  - O que é ORM
    - Object Relational Mapping, em português, mapeamento objeto relacional
    - É um recurso para aproximar o paradigma da orientação a objetos ao contexto de banco de dados relacional
    - O uso de ORM é realizado através do mapeamento de objeto para uma tabela por uma biblioteca ou framework
  - Java Persistence API
    - É uma especificação baseada em ‘interfaces’
    - Através de um framework realiza operações de persistência de objetos em Java
    - Hibernate, EclipseLink, TopLink, OpenJPA
  - Mapeamentos
    - Identificação
    - Definição
    - Relacionamento
    - Herança
    - Persistência
  - EntityManager
    - É uma estrutura de camadas para acessar os dados no banco de dados
- Spring Data JPA
  - CrudRepository
  - JPARepository
  - PagingAndSortingRepository
  - @Query
  - @Param
  - Com o Spring Data JPA não é mais necessário configurar o repository
  - Ele já oferece o repository pronto criando uma interface que que extende o repository
- Conexão com Postgres
  - Todas as configurações para conectar com o Postgres
  - Tomar cuidado com o nome da classe como User, pois é uma tabela reservada do banco de dados
- JPA repository
  - O DAO era utilizado antes do repository
  - O repository já traz todas as operações de um CRUD
  - Para consultas customizadas pode-se utilizar Query Method ou Query Override
  - Query Method
    - Utiliza JPQL
    - O nome do método é utilizado como se fosse uma query do banco de dados
  - Query Override
    - Utilizado para consultas nativas
    - Bom quando o nome da Query Method fica muito grande

#### Conclusão
- Conclusão e para saber mais
  - Dominamos o Spring Boot Framework
  - Criamos um projeto
  - Exploramos o IoC / DI
  - Conhecemos a central de propriedades
  - Interagimos com o banco de dados

### Criando uma API REST Documentada com Spring Web e Swagger

#### Apresentação Inicial
- Apresentação e visão geral do curso
  - Criar uma API REST documentada com Spring Web e Swagger
  - Criar um projeto Web
  - Configurando Controllers
  - Documentar a API com Swagger
  - Tratamento de exceções com Handlers

#### Projeto Spring Boot
- Criando uma REST API
- RestController
- Documentando a nossa API com SWAGGER
- Habilitando o tratamento de exceções de negócio com handlers

#### Conclusão
- Conclusão e para saber mais

### Criando uma API REST com Spring Security

### Explorando Padrões de Projetos, na Prática com Java

### Desafios de código Java intermediários: Design Patterns

### Aula Inaugural - Java AI Powered

## Explorando Testes e Arquiteturas Java de Alta Escalabilidade

### Introdução a Testes de ‘software’

### Testes Unitários com JUnit

### Desenvolvendo testes utilizando Mockito

### Introdução aos conceitos de API e Clean Architecture

### Introdução a Arquitetura Hexagonal com Spring Boot e Kotlin

### Desmistificando microserviços, BFF e `DDD`

### Arquitetura Orientada a Eventos com Java, Spring Boot e Kafka

### Desenvolvendo um sistema para eleição usando Quarkus Framework

### Desafios de Código Java intermediários: S.O.L.I.D

## AWS Cloud Computing para `soluções Java`

### Criando a sua conta na AWS

### Introdução ao conceito de `Cloud`

### Infraestrutura Global AWS

### Computação em AWS

### Redes em AWS

### Armazenamento e banco de dados AWS

### Redução de custos em farmácias com AWS

### Publicando sua API REST na nuvem usando Spring Boot 3, Java 17 e Railway

### Avalie este Bootcamp
