# Lojinha Automação API

Esse é um repositório que contém a automação de alguns testes de API Rest de um software denominado Lojinha. Os tópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas

- Java https://www.oracle.com/java/technologies/downloads/
- JUnit https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine
-  RestAssured https://mvnrepository.com/artifact/io.rest-assured/rest-assured/4.4.0
- Maven
  https://mvnrepository.com/

## Testes Automatizados

- Testes para validar as partições de equivalência relacionadas ao valor do produto na Lojinha, que estão vinculados diretamente a regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$7.000,00.


## Notas Gerais

- Sempre utilizada a anotação Before Each para capturar o token que será utilizados posteriormente nos métodos de testes.
- Armazenado os dados que são enviados para a API através do uso de classes POJO.
- Criado dados iniciais através do uso de classes Data Factory, para facilitar a criação e controle dos mesmo.
- Nesse projeto foi usado o JUnit 5, o que dá a possibilidade de usar a anotação Display Name para dar descrições em português para os testes.
