# Lojinha Automação API

Este projeto consiste em um conjunto de testes automatizados para a API REST da aplicação "Lojinha". Ele foi desenvolvido para validar endpoints específicos e garantir a integridade dos dados e funcionalidades da API.

## Tecnologias Utilizadas

- **Java**: Linguagem principal para os testes.
- https://www.oracle.com/java/technologies/downloads/
- **JUnit 5**: Framework para execução de testes unitários e de integração.
- https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine
-  **Rest-Assured**: Biblioteca para testes de API RESTful em Java. https://mvnrepository.com/artifact/io.rest-assured/rest-assured/4.4.0
- **Maven**: Gerenciador de dependências e automação de build.
  https://mvnrepository.com/

## Estrutura do Projeto

-   **`ProdutoTest.java`**: Classe que contém os testes para os endpoints da API REST relacionados ao módulo de produtos.
-   **`UsuarioDataFactory.java`**: Classe utilitária para criar usuários com diferentes perfis (exemplo: administrador).
-   **`ProdutoDataFactory.java`**: Classe utilitária para criar produtos com configurações específicas.
-   **`Pojo`**: Classes que representam os objetos enviados e recebidos nas requisições (exemplo: `ComponentePojo`, `ProdutoPojo`, `UsuarioPojo`).


## O que foi feito

-   Configuração de uma base URI e basePath para facilitar a execução de testes nos endpoints da API.
-   Obtenção do token de autenticação do administrador via endpoint de login para utilização nos testes.
-   Implementação de testes para os endpoints do módulo de produtos, incluindo:
  -   Criação de produtos.
  -   Validação de dados retornados pela API.
  -   Tratamento de respostas HTTP e validação de status codes.
- Dados que estão vinculados diretamente a regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$7.000,00.

## Notas Gerais

- Sempre utilizada a anotação Before Each para capturar o token que será utilizados posteriormente nos métodos de testes.
- Armazenado os dados que são enviados para a API através do uso de classes POJO.
- Criado dados iniciais através do uso de classes Data Factory, para facilitar a criação e controle dos mesmo.
- Nesse projeto foi usado o JUnit 5, o que dá a possibilidade de usar a anotação Display Name para dar descrições em português para os testes.

## Contribuição
Contribuições são bem-vindas! 
Sinta-se à vontade para abrir issues ou enviar pull requests.
