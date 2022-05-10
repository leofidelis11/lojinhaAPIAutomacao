# Lojinha API Automação
Esse é o repositório que contém a automação de alguns testes de API Rest de um software denominado Lojinha. Os subtópicos abaixo descrevem algumas decisões tomadas na estruturação do projeto.

## Tecnologias Utilizadas
- Java
  https://www.oracle.com/java/technologies/downloads/
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine
- Rest Assured
  https://mvnrepository.com/artifact/io.rest-assured
- Maven
  https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalências relacionadas ao valor do produto na Lojinha que estão vinculados diretamente a regra de negocio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais
- Sempre utilizamos a anotação Before Each para capturar o token que será utilizado posteriormente nos métodos de teste.
- Armazenamos os dados que são enviados para a API através do uso de classes POJO.
- Criamos dados iniciais através do uso de classes DataFactory, para facilitar a criação e controle dos mesmos.
- Nesse projeto fazemos uso do JUnit 5, o que nos dá a possibilidade de usar a anotação DisplayName para dar descrições em português para nossos testes.