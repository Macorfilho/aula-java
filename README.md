# Aula Java

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)
![Status: estudo](https://img.shields.io/badge/status-estudo-blueviolet?style=for-the-badge)

## Visão Geral

Projeto de estudo da disciplina **3ECB — FIAP**, criado no Spring Initializr como introdução ao desenvolvimento de aplicações web com **Spring Boot**. O projeto demonstra o primeiro passo no framework: uma aplicação contendo dois controllers REST simples — um endpoint de saudação em português e um endpoint de cálculo de soma entre dois números.

## Tecnologias Utilizadas

| Categoria | Tecnologia | Uso no projeto |
|---|---|---|
| Linguagem | Java 17 | Lógica das rotas |
| Framework | Spring Boot 3.4.2 | Estrutura da aplicação web |
| Build | Maven | Compilação, dependências e execução |

## Arquitetura & Funcionalidades

**Funcionalidades implementadas:**

- `GET /hello` — retorna a mensagem "Olá, Spring Boot!".
- `GET /calculo/soma/{num1}/{num2}` — retorna a soma de dois números inteiros informados na URL.

## Instalação e Configuração

**Pré-requisitos:**

- JDK 17+
- Maven (ou use o `./mvnw` fornecido)

```bash
git clone git@github.com:Macorfilho/aula-java.git
cd aula-java
./mvnw clean package
```

Não há variáveis de ambiente ou configurações adicionais — apenas `spring.application.name=aula-java` em `application.properties`.

## Como Executar / Exemplos de Uso

```bash
./mvnw spring-boot:run
```

```bash
# Saudação
curl http://localhost:8080/hello
# → Olá, Spring Boot!

# Soma
curl http://localhost:8080/calculo/soma/5/7
# → 12
```

## Contato / Créditos

Desenvolvido por Marcelo R. Corner Filho.

- Portfólio: https://marcelocorner.dev
- GitHub: https://github.com/Macorfilho
- LinkedIn: https://www.linkedin.com/in/marcelocorner