# <h1>poc-kafka</h1>
<h2>O objetivo deste projeto é compartilhar os conhecimentos de Kafka entre a squad</h2>


<h2><b>Primeira Etapa</b></h2>

<p>1 - Subir um docker-compose com o zookeeper, kafka e uma interface para visualização do Kafka.</p>
<p>2 - Criar um projeto que deve produzir mensagens para um tópico Kafka.</p>
<p>3 - Criar um projeto que deve consumir mensagens de um tópico Kafka.</p>

<b>Requisitos:</b>
 - Para essa primeira etapa, sugiro utilizar as dependências:
 
     <dependency>
       <groupId>org.apache.kafka</groupId>
       <artifactId>kafka-streams</artifactId>
    </dependency>

    <dependency>
       <groupId>org.springframework.kafka</groupId>
       <artifactId>spring-kafka</artifactId>
    </dependency>

    <dependency>
      <groupId>org.springframework.boot</groupId>
      <artifactId>spring-boot-starter-web</artifactId>
    </dependency>

    <dependency>
      <groupId>com.h2database</groupId>
      <artifactId>h2</artifactId>
      <scope>runtime</scope>
    </dependency>
    
 <b>Critérios de Aceite:</b>

 - Para o primeiro objetivo, ao subir o docker-compose, deve subir também um arquivo .txt com os comandos básicos para criar um tópico, produzir uma mensagem, consumir uma mensagem e listar todos os tópicos.
 - Para o segundo objetivo, o projeto que contém o producer deve conter um endpoint que quando chamado, ele deve produzir uma mensagem no tópico com as informações do request.
 - Para o terceiro objetivo, o projeto que contém o consumer deve consumir a mensagem e perstir em um banco de dados relacional ou não.
 
 
 
 <b>Dicas:</b>
 - A própria documentação do Spring kafka já passa o básico para criação de um producer e consumer.
 - Tenho esse repo com as implementações do kafka que vocês podem se basear nele: 
  - o primeiro é projeto que contem um producer e o consumer
  - o segundo é só o producer
  - o terceiro é só o consumer
  LINK: https://github.com/Bodegami/apache-kafka-spring
