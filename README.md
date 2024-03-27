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
  - REST é um guia de boas práticas
  - RESTFul é a capacidade de determinado sistema aplicar os princípios de REST
    - Cliente/Servidor
    - Interface uniforme
    - Stateless
    - Cache
    - Camadas
  - Nível de maturidade
    - Definido em 4 níveis
    - Level 0 The swamp of POX -> Ausência de regras
    - Level 1 Resources -> Define os nomes dos recursos e define os verbos
    - Level 2 Http Verbs -> Valida a aplicabilidade dos verbos
    - Level 3 Hypermedia Controls -> HATEOAS
    - Glory of REST
- RestController
  - Uma classe contendo anotações específicas para a disponibilização de recurso HTTP baseados nos nossos serviços e regras de negócio
- Documentando a nossa API com SWAGGER
  - É um centralizador de API
  - Atualmente basta adicionar uma dependência 
  ```
  <dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.3.0</version>
  </dependency>
  ```
  - E acessar a URL http://localhost:8080/swagger-ui/index.html#/
- Habilitando o tratamento de exceções de negócio com handlers
  - Conseguir ajudar o usuário a entender o problema
  - Pode Utilizar o ControllerAdvice
  - Pode utilizar o ExceptionHandler em cada método
  - Pode utilizar o ResponseStatusExceptionResolver
  - Pode utilizar o RestControllerAdvice
    - Centraliza num único componente todas as exceções
    - Existem formas melhores de fazer o controle de exceção
    - A centralização das exceções de campo requerido foi boa

#### Conclusão
- Conclusão e para saber mais
  - Criamos um projeto WEB
  - Estruturamos nossos controllers
  - Documentamos a nossa API
  - Habilitamos tratamento de exceções
  - Interagimos com a API via Postman

### Criando uma API REST com Spring Security

#### Apresentação Inicial
- Apresentação e visão geral do curso
  - Spring Boot Security
  - Introdução sobre segurança
  - Habilitando segurança com spring
  - Configure Adapter
  - Autenticação com banco de dados
  - JWT - Json Web Token

#### Spring Boot Security com JWT
- Habilitando segurança com Spring
  - É apenas um grupo de filtros servlet que ajudam você a adicionar autenticação e autorização ao seu aplicativo ‘web’
  - É configurado um utilizador e senha padrão, quando se cria um projeto com spring security
  - Utilizar: user
  - Senha: gerada a cada execução do projeto
- Autenticação simples
  - É feita no application.properties
  ```
  spring.security.user.name=user
  spring.security.user.password=user123
  spring.security.user.roles=USERS
  ```
  - Tem como gerar mais de um utilizador em memória
  - O curso está com código desatualizado
- Configure Adapter
  - Centraliza as configurações de acesso a recursos
  - O curso está com código desatualizado
  - A versão mais recente do spring security é de fevereiro de 2024 nesse momento
- Autenticação com Banco de dados
  - Foi utilizado o banco `H2`
  - O curso está com código desatualizado
  - A parte mais difícil foi criar um componente separado para a geração do encode da senha
- JWT - JSON Web Token - Parte 1
  - É um JSON com as informações do utilizador da aplicação
  - Constituído por um `Header`, `Payload` e `Signature`
- JWT - JSON Web Token - Parte 2
  - Adicionando dependência do JWT
  - Pacotes da aplicação
    - model
    - dto
    - repository
    - service
    - controller
    - security
  - Classes da aplicação
    - SwaggerConfig — Não precisa mais porque a dependência já configura para nós
    - JWTObject
    - JWTCreator
- JWT - JSON Web Token - Parte 3
  - Configuração antiga de 2022
  - Precisa utilizar o Java 8 e algumas dependências do maven para funcionar
- JWT - JSON Web Token - Parte 4
  - Testes com o JWT
  - Banco de dados não funcionou para acessar o `H2`

#### Conclusão
- Conclusão e para saber mais
  - Habilitamos a segurança na nossa API
  - Conhecemos algumas formas de configurar segurança
  - Configuramos manualmente a segurança da nossa API
  - Consultamos os nossos utilizadores em banco de dados
  - Melhoramos a segurança da nossa API com JWT

### Explorando Padrões de Projetos, na Prática com Java
- Como usar os desafios de projeto para criar o seu `portfolio`
  - Explicação de como entregar os desafios
- Apresentação Inicial
  - Os padrões de projeto serão feitos com Java Puro
  - Alguém está sentado na sombra hoje porque alguém plantou uma árvore há muito tempo `Warren Buffet`
- Padrões de projeto
  - Passo 1 — Padrões de Projeto
  - Passo 2 — Praticando com Java Puro
  - Passo 3 — Praticando com Spring
  - Passo 4 — Desafio de Projeto
  - A principal referência foi feita em 1995 no livro `Design Patterns: Elements of Reusable Object-Oriented Software`
  - Divido em:
    - Criacionais
    - Comportamentais
    - Estruturais
  - Falar é fácil. Mostre-me o código `Linus Torvalds`
- Praticando com Java Puro: Singleton
  - Permitir a criação de uma única instância de uma classe e fornecer um modo para recuperá-la
- Praticando com Java Puro: Strategy
  - Simplificar a variação de algoritmos para a resolução de um mesmo problema
- Praticando com Java Puro: Facade
  - Prover uma ‘interface’ que reduza a complexidade nas integrações com subsistemas
- Praticando com Spring: Introdução
  - Relacionar padrões de projeto com o Spring
  - Singleton: @Bean e @Autowired
  - Strategy: @Service e @Repository
  - Facade: Spring Data JPA e ViaCEP
- Praticando com Spring: Conhecendo o Projeto Base
  - CrudRepository é uma Strategy
- Praticando com Spring: Padrões de Projeto numa API REST
  - Desenvolvendo o repository do cliente
  - Testando a API
  - Funcionou tudo corretamente
- Desafio de Projeto
  - Pelo que entendi é para criar um projeto com algum `design patterns`
  - Vou usar o meu projeto com todos os `design patterns`
- Entendendo o desafio
  - Entregar um projeto com algum `design pattern` implementado
  - Entreguei o meu repositório com o estudo sobre todos os `design pattern` do GoF

### Desafios de código Java intermediários: Design Patterns
- Algumas questões sobre `Design Patterns`
- Todas as questões foram respondidas na plataforma

### Aula Inaugural - Java AI Powered
- Autodescrição é uma coisa ótima nos vídeos
- Curso voltado para quem quer trabalhar fora do Brasil
- Curso voltado para utilizar IA na programação
- Vídeo de 1 hora e meia
- O recomendado são 10 horas por semana
- As empresas buscam por especialistas

## Explorando Testes e Arquiteturas Java de Alta Escalabilidade

### Introdução a Testes de ‘software’
- Introdução
  - Introdução
    - Apresentação do instrutor do curso
    - Atua desde 2012
    - Entender o que é testes de software e seus principais conceitos
    - Compreender como essa disciplina permeia o desenvolvimento de ‘software’
    - Entender os diversos testes e as suas finalidades
    - Falar um pouco sobre qualidade de ‘software’
    - Definição e conceitos básicos
    - Níveis e técnicas de teste
    - Testes não funcionais
    - A pirâmide de testes
- Definição e conceitos básicos
  - Definição de Testes
    - Evitar que o cliente final utilize outro sistema por questão de erro
    - Como testar?
      - Valor -> Saque -> Resultado
    - Erros em produção são muito caros
    - Chega a casa dos milhões
    - Definição (Dias Neto)
      - É o processo de execução de um produto para determinar se ele atingiu as suas especificações funcionou corretamente no ambiente para o qual foi projetado
    - Definição (Edsger W. Dijkstra)
      - Testes podem ser usados para mostrar a presença de erros, mas nunca para mostrar a sua ausência
  - Evolução de Testes na engenharia de ‘software’
    - Cascata
      - Especificação
      - Projeto de software
      - Implementação
      - Testes
      - Implantação
    - Desenvolvimento ágil
      - Meet & Plan
      - Design
      - Code & Test
      - Release
      - Feedback
  - Conceitos básicos
    - Defeito: É o erro do sistema ou `Bug`
    - Erro: Com o desenvolvedor
    - Falha: Com o utilizador final
    - Verificação: Verificar se o sistema está construido da forma correta
    - Validação: Verificar se as regras de negócio estão corretas
- Níveis e técnicas de teste
  - Níveis de teste
    - Unidade
      - JUnit
    - Integração
      - Testar os componentes entre si
      - Banco de dados
      - API
      - Entre outros
    - Sistema
      - Testar num ambiente de homologação
      - Somente para alguns utilizadores
    - Regressão
      - Testar se as novas features não irão quebrar as features existentes
      - Utiliza o Selenium
    - Alpha: Com certeza vai ter algo para ajustar 
    - Beta: Já está próximo do que é esperado 
    - Cannary 
      - Deploy canário
      - Somente algumas pessoas têm acesso às novas versões
    - Aceitação
      - Já foi para produção
      - Antigamente era mais formal
      - BDD automatizou esse processo
  - Técnicas de teste
    - Cada nível de teste possui técnicas diferentes
    - Caixa Branca
      - Também conhecida como teste estrutural
      - Validar dados, controles, fluxos, chamadas
      - Garantir a qualidade da implementação
      - Níveis: Unidade, Integração e Regressão
    - Caixa Preta
      - Teste funcional
      - Verificar saídas usando várias entradas
      - Teste sem conhecer a estrutura interna do ‘software’
      - Níveis: Integração, Sistema e Aceitação
    - Caixa Cinza
      - Mescla técnicas de caixa branca e caixa preta
      - Analisa parte lógica e também funcionalidade
      - Exemplo: ter acesso à documentação do funcionamento do código
      - Engenharia reversa
- Testes não funcionais
  - O que são testes não funcionais
    - Testes não funcionais estão ligados a requisitos não funcionais
      - Comportamento do sistema
      - Performance
      - Escalabilidade
      - Segurança
      - Infraestrutura
    - Testes não funcionais visa testar partes do ‘software’ que não são associados as regras de negócio, mas sim a requisitos não funcionais
    - São utilizadas ferramentas que usam técnicas para apurar o comportamento do sistema em determinadas circunstâncias
    - Teste de carga
      - Realizado para verificar qual o volume de transações, acessos simultâneos ou utilizadores que um servidor/‘software’/sistema suporta
      - Pontos de atenção
        - Objetivos para clareza de resultados
        - Ambiente
        - Cenários
        - Execução de testes
        - Análise de resultado
      - Gattling Load Testing
      - Apache JMeter
    - Teste de estresse
      - Realizado para submeter o ‘software’ a situações extremas
      - O teste de estresse baseia-se em testar os limites do ‘software’ e avaliar o seu comportamento
      - Avalia-se até quando o ‘software’ pode ser exigido e quais as falhas decorrentes do teste
      - Apache JMeter
    - Teste de segurança
      - É um processo crítico de segurança cibernética que visa encontrar vulnerabilidades em sistemas, ‘software’, redes e aplicativo
- A pirâmide de testes
  - A pirâmide de testes
    - Testes unitários (rápido e isolado)
    - Testes de serviços (mediano e isolado medianamente)
    - Testes de `UI` (demorado e integrado)
    - Software Testing Ice Cream Cone Anti-Pattern
      - Testes manuais
      - Testes automatizados
      - Testes de integração
      - Testes unitários
    - Tente fugir desse pattern
- Encerramento
  - Encerramento
    - É um curso somente de introdução para ter uma base sobre testes de ‘software’
    - Conceitos básicos e a evolução da disciplina de testes
    - Terminologia
    - Níveis e técnicas de teste
    - Testes não funcionais
    - Pirâmide de testes

### Testes Unitários com JUnit
- Apresentação do curso
  - Apresentação do curso
    - Entender a motivação de escrever testes unitários
    - Conhecer o que é o JUnit
    - Configurar a ferramenta para utilizar nos seus projetos java
    - Aprofundar nos recursos que ele provê para construir testes unitários efetivos
    - Por que escrever testes unitários?
    - Hello World, Junit!
    - Aprofundando nos recursos
    - Recursos das IDEs
    - Boas práticas
    - Conclusão
- Por que escrever testes unitários
  - Por que escrever testes unitários
    - Entender o que é teste unitário e a sua importância
    - O que são testes unitários?
      - Também chamado teste de unidade
      - Testar a menor unidade de código possível
      - Unidade: função, método, classe
      - Testar uma aplicação na sua menor parte
      - Geralmente escrito em tempo de desenvolvimento
    - Exemplo simples demonstrado
    - Por que escrever testes unitários?
      - Compreender o código fonte
      - Corrigir erros com segurança
      - Refatorar código sem introduzir erros
      - Entregar com segurança uma nova versão
      - Pirâmide de testes
      - Testes unitários como métrica de qualidade (confiabilidade)
      - Cobertura de testes
      - Automação na execução de testes
      - Cultura de agilidade
- Hello World, JUnit
  - Hello World, Junit
    - Falar um pouco sobre a história do JUnit
      - Ferramenta de código aberto para criação de testes unitários 
      - Criado por Erich Gamma e Kent Beck
      - Kent Beck é o criador do TDD
      - Erich Gamma faz parte da `Gang of Four` que criou o conceito de Padrões de Projeto
    - Falar um pouco sobre a versão atual
      - Versão atual 5
      - Junit Platform
        - É o componente que executa os testes
      - JUnit Jupiter
        - Todas as classes e interfaces ficam dentro dele
      - JUnit Vintage
        - Faz integração com as versões anteriores
    - Configurar em projeto Maven e Gradle a ferramenta
      - Basta adicionar a dependência
- Aprofundando nos recursos
  - O básico para testar
    - Conhecer em detalhes os pricipais recursos que o JUnit provê
  - Mais algumas asserções
    - Algumas dicas para testes
  - After e Before
    - All: executado depois que todos os testes forem finalizados
    - Each: executado em cada teste
  - Assumptions e testes condicionais
    - Assumptions: Os testes são executados somente se a Assumption estiver correta
  - Testando exceptions
    - assertThrows e assertDoesNotThrows
  - Ordenando testes
    - OrderAnnotation
    - MethodName
    - Random
    - DisplayName
- Recursos de testes nas IDEs
  - Conhecer o básico para executar testes unitários nas IDEs mais utilizadas pelo mercado
  - Visual Studio Code
    - É possível executar testes no VS Code
    - Precisa instalar uma extensão
  - Eclipse
    - O eclipse é mais bonito as execuções de teste
    - Podemos dizer que traz mais detalhes dos testes
    - Tem como definir o valor de algumas variaveis
  - Intellij IDEA
    - A interface do Intellij é mais limpa
    - Também aceita realizar debug no código
- Boas práticas
  - Boas práticas
    - Conhecer boas práticas adotadas ao escrever testes unitários
    - Preocupe-se com os nomes
    - Preocupe-se com a facilidade de leitura
    - Procure escrever o código de teste o mais próximo possível do código de execução
    - Veja um pouco sobre TDD
      - Escreva um teste que falhe
      - Faça o código funcionar
      - Elimine redundância
    - Busque uma padronização de nomenclatura
    - Testes precisam ser determinísticos
      - Um teste não pode influenciar no outro
    - Economize tempo automatizando
      - Ferramentas de cobertura de código (JaCoCo)
      - Automatize a execução dos seus testes
- Conclusão do curso
  - Conclusão do curso
    - Motivação
    - Configuração
    - Principais recursos
    - Usando os recursos das IDEs
    - Boas práticas

### Desenvolvendo testes utilizando Mockito
- Apresentação do curso
- Introdução ao Mockito
- Mockando objetos
- Espiando objetos
- Capturando argumentos
- Manipulando retornos
- Mockando métodos estáticos
- Conclusão

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