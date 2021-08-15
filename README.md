# Fazendo testes com JUnit
## Pré-requisitos
- Java JDK 8 ou posterior instalado.
- Maven instalado.
- Um IDE ou editor de textos avançado (IntelliJ, Eclipse, Visual Studio Code).
- Obs: O JUnit foi adicionado nas dependências do projeto.

## O que é um framework de testes?
- Ferramenta que permite acelerar, facilitar ou organizar o processo de testes, normalmente no contexto de automatização. 
- Conjunto de regras ou diretrizes utilizadas para definir um processo de trabalho de testes.

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
`mvn clean compile test`: É um comando para executar no terminal, onde mostra todos os testes. <br>
`assertEquals();`: Recebe um valor esperado e um valor objeto, depois checa se eles são iguais, se forem iguais não faz nada, se não forem dispara uma exceção.

## Dicas
- Se o método tem mais de 10 linhas, reveja.
- Se o método tem mais de 20 linhas, refatore.
