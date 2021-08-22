# Fazendo testes com JUnit
## Pré-requisitos
- Java JDK 8 ou posterior instalado.
- Maven instalado.
- Um IDE ou editor de textos avançado (IntelliJ, Eclipse, Visual Studio Code).
- Obs: O JUnit foi adicionado nas dependências do projeto.

## O que é um framework de testes?
- Ferramenta que permite acelerar, facilitar ou organizar o processo de testes, normalmente no contexto de automatização. 
- Conjunto de regras ou diretrizes utilizadas para definir um processo de trabalho de testes.

## Como executar os testes?
>mvn clean compile test

## Exemplos de frameworks de testes
- JUnit (mais básico).
- TestNG (concorrente do JUnit, mais básico).
- e-FATHREE (framework da Everis, mais avançado).
- Selenium (abstrai o acesso ao navegador para realizar automações web).
- Obs: é possível usar mais de um framework nos seus testes.

## Principais benefícios de utilizar um framework
- Maios eficiência.
- Maior velocidade na criação dos testes.
- Menor custo de manutenção.
- Maior cobertura de testes.
- Reutilização do código.

## Extensão para o Visual Studio Code
O nome da extensão é `Java Extension Pack`, com ela é possível ver os testes que passaram e falharam.

## Boas práticas que aprendi com JUnit
`@Test`:  Mostra que um método é de teste. É uma annotation, pois vem acima do método e é inicializada com @. <br>
`@Disabled`: Não executa o teste que essa annotation foi declarada. <br>
`@BeforeAll`: Define um código que vai ser executado antes dos testes (exemplo, instanciar objetos). <br>
`@BeforeEach`: Roda o código antes de cada teste. <br>
`@AfterEach`: Roda depois de cada teste. <br>
`@AfterAll`: É executado apenas 1 vez, é executado por último. <br>
`@DisplayName();`: Adiciona um nome para o teste. <br>
`@ParameterizedTest`: Diz que o próximo teste recebe parâmetros. <br>
`@CsvSource({})`: Indica que o parâmetro é do tipo csv. <br>
`@CsvFileSource(resources = "/data.csv", numLinesToSkip = 1)`: Indica que o arquivo é do tipo csv. Passou o path do arquivo e as linhas para pular. <br>
`fail();`: Usado em condicionais para mostrar uma mensagem de falha. <br>
`assertEquals();`: Recebe um valor esperado e um valor objeto, depois checa se eles são iguais, se forem iguais não faz nada, se não forem dispara uma exceção.

## Asserts
- Define se um caso de teste foi sucesso ou não.
- [Assert.assertEquals()](https://www.guru99.com/junit-assert.html)

Como usar:
>import static org.junit.Assert.*;

## Dicas
- Se o método tem mais de 10 linhas, reveja.
- Se o método tem mais de 20 linhas, refatore.

## Documentação
- [Mockito e JUnit5](https://www.baeldung.com/mockito-junit-5-extension)
- [Mockito](https://site.mockito.org/)
- [Hamcrest](http://hamcrest.org/)
- [Matcher](https://docs.oracle.com/javase/7/docs/api/java/util/regex/Matcher.html)
- [AssertJ](https://assertj.github.io/doc/)

## Perguntas e respostas
### O que são Mocks?
Tipos primitivos, Objetos e Arrays.

### O framework Mockito permite que:
Sejam construídos testes com uma API simples e clara.

### Qual Matcher permite inspecionar classes da API de Collection?
Collection Matcher

### Por que usar Mocks? 
Uma das razões para usar Mocks é que criar objetos reais para testes é difícil.

### O Matcher greaterThan verifica se:
Verifica se o valor atual é maior que o esperado.

### O que é AssertJ?
Um framework usado para escrever Assertions mais fluentes.

### AssertEquals verifica se:
O valor esperado e atual são iguais.

### Asserts são fornecidos por qual classe?
org.junit.Assert

### PowerMockito é uma API de extensão que permite trabalhar com:
Reflection.

## Sobre a Autora
Oi, eu sou a Fernanda! Estou aqui para contribuir com meu conhecimento e espero poder ajudar no desenvolvimento profissional de cada um de vocês.

[![Linkedin Badge](https://img.shields.io/badge/-Fernanda_Maki_Hirose-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)](https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)  [![Gmail Badge](https://img.shields.io/badge/-femahi2020@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:femahi2020@gmail.com)](mailto:femahi2020@gmail.com)
