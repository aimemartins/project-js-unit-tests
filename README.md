# Projeto Zoo Functions

Esse projeto foi elaborado durante o Módulo de Fundamentos do curso da Trybe para desenvolver habilidades com os conteúdos e tecnologias de: <br>
<br>
🔹 JavaScript versão ES6 <br>
🔹 Testes Unitários <br>

 ###### :warning: Importante <br> <br> Apenas os arquivos indicados nos requisitos foram desenvolvidos pelo(s) aluno(s), os demais são de autoria da Trybe.

## Índice
- [Elaboração](#elaboração)
- [Sobre](#sobre)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Instalação](#instalação)
- [Testes](#testes)
- [Requisitos](#requisitos)
   - [Requisitos Obrigatórios](#requisitos-obrigatórios)
   - [Requisitos Bônus](#requisitos-bônus)
- [Progresso](#progresso)


## Elaboração
<a href="https://github.com/aimemartins">
  <img src="https://avatars.githubusercontent.com/u/108954069?v=4" width="80px" alt="Aimê Martins"/> <p>Aimê Martins</p>


## Sobre

Você implementará várias funções na resolução dos requisitos propostos e/ou testes unitários para garantir que as implementações das funções estão corretas, de acordo com o que está sendo solicitado em cada enunciado.

Nesse projeto, você será capaz de:

- Escrever testes unitários utilizando o módulo Jest do NodeJS para verificar o correto funcionamento das funções;
- Escrever funções de forma que elas atendam a testes já implementados;
- Escrever testes e funções utilizando uma abordagem de desenvolvimento orientado a testes.

## Estrutura do Projeto

As funções a serem implementadas estão dentro da pasta `src` e seus respectivos testes estão na pasta `tests`. O nome dos arquivos também segue uma ordem definida. Basicamente, os arquivos de teste possuem o nome do arquivo alvo (arquivo da funcionalidade) acrescido do nome `.spec.js`.

Há um arquivo como `src/exemplo.js` que contém a implementação de uma função e um arquivo como tests/exemplo.spec.js com os testes unitários referentes à função presente no arquivo `src/exemplo.js`.

Cada função possui um bloco de comentários em suas primeiras linhas explicando qual é o trabalho que a função deve realizar.

## Instalação

1. Clone o repositório com o comando: `git clone git@github.com:tryber/project-js-unit-tests.git`
2. Entre na pasta do repositório que você acabou de clonar: `cd project-js-unit-tests`
3. Execute o comando `npm install` para instalar as dependências.
   
## Testes

Todos os requisitos do projeto serão testados automaticamente por meio do `Jest`.

Os comandos que você utilizará com mais frequência são:

`npm test` (executa todos os testes presentes na aplicação)
`npm test caminho/para/arquivo` (executa apenas os testes presentes no arquivo especificado)
Exemplo: `npm test tests/average.spec.js`


## Requisitos 
   
   ### Requisitos Obrigatórios
   
   1. Implemente a função `average`.
      - A função `average` recebe um array de tamanho variável e retorna a média dos valores recebidos. Caso a função receba algum valor não numérico ou um array vazio, o valor `undefined` deve ser retornado.
        
   2. Implemente os casos de teste para a função `numbers`.
      - A função `numbers` recebe um array de tamanho variável e retorna `true` se todos os parâmetros forem do tipo 'number' e `false` caso contrário.
        
   3. Implemente a função `vqv`.
      - Use template literals para escrever a função `vqv` que recebe o seu nome e a sua idade e retorna o parágrafo descrito abaixo:
        <br>
         `Oi, meu nome é Tunico!
        Tenho 30 anos,
        trabalho na Trybe e mando muito em programação!
        #VQV!`
        <br>
   4. Implemente os casos de teste para a função `circle`
      - A função `circle` recebe o raio de um círculo e retorna um objeto contendo as suas informações: Raio, Área e Circunferência. Se não for especificado um raio, a função retorna `undefined`.
        
   5. Implemente a função `createStudent`
      - A função `createStudent` recebe como parâmetro um **nome**, e retorna um objeto contendo duas chaves: <br>
<br>
          - 1. name, contendo o nome passado como parâmetro; <br>
          - 2. feedback, contendo uma função que retorna a frase "Eita pessoa boa!" ao ser chamada. <br>
      - O arquivo `createStudent.spec.js` contém os testes para `createStudent` já implementados. Implemente a               função no arquivo `src/createStudent.js` de forma que ela atenda aos testes propostos.
<br>
<br>
        
   6. Implemente os casos de teste para a função `productDetails`.
      - A função `productDetails` recebe duas strings que representam nomes de produtos, e retorna um array contendo dois objetos com os detalhes dos respectivos produtos:
          - productDetails('Alcool gel', 'Máscara');
          - Retorna: [
  {
    name: 'Alcool gel'
    details: {
      productId: 'Alcool gel123'
    }
  },
  {
    name: 'Máscara'
    details: {
      productId: 'Máscara123'
    }
  }
]
<br>
Essa função já está implementada no arquivo src/productDetails.js. Escreva pelo menos cinco testes para essa função no arquivo tests/productDetails.js para garantir que a implementação de productDetails está correta.
      <br>
   7. Implemente as funções calculator e `arrayGenerator`.
      - A função `calculator` recebe dois números inteiros como parâmetro e retorna um objeto com as seguintes chaves:

- sum; - mult; - div; - sub.
Para cada chave atribua como valor a operação correspondente à sua chave:

sum: retorna o resultado da soma dos dois números;
mult: retorna o resultado da multiplicação dos dois números;
div: retorna o resultado da divisão dos dois números;
sub: retorna o resultado da subtração dos dois números.
Os resultados das divisões devem sempre ser arredondados para baixo.

Parâmetros:

Dois números inteiros.
Comportamento:

calculator(1, 2); // { sum: 3, mult: 2, div: 0, sub: -1 }
Já a função arrayGenerator converte objetos em arrays, de chaves, valores ou ambos. Ela deve receber dois parâmetros:

o primeiro parâmetro deve ser uma string que indica o tipo de conversão;
o segundo parâmetro deve ser um objeto semelhante ao que é retornado pela função calculator que você acabou de desenvolver.
Parâmetros:

Uma string que indica o tipo de conversão;
Um objeto no formato { sum: 3, mult: 2, div: 0, sub: -1 };
Comportamento:

arrayGenerator('keys', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 'sum', 'mult', 'div', 'sub' ]
arrayGenerator('values', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 3, 2, 1, 0 ]
arrayGenerator('entries', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ [ 'sum', 3 ], [ 'mult', 2 ], [ 'div', 1 ], [ 'sub', 0 ] ]
O arquivo objPlayground.spec.js contém os testes para calculator e arrayGenerator já implementados. Implemente as funções no arquivo src/objPlayground.js de forma que ela atenda aos testes propostos.


      
   8. Implemente a função ´myCounter`.
      - A função `myCounter` possui dois loops aninhados que inserem valores dentro de um array. Como podemos perceber, eles vão adicionando valores ao array até sua condição de parada.
       
   9. Implemente os casos de teste para a função `getCharacter`.
          - A função `getCharacter` recebe uma string que representa o nome de uma personagem e retorna um objeto contendo o seu nome, a sua classe e as suas frases.
            
   10.  Implemente a função `createMenu`, bem como seus casos de teste
       - Esse último requisito vai guiar você por um rico processo de Desenvolvimento Orientado a Testes ou TDD - Test Driven Development.
         
## Progresso
O projeto está em andamento 🚧


# :construction: README em construção ! :construction:
<!-- Olá, Tryber!
Esse é apenas um arquivo inicial para o README do seu projeto.
É essencial que você preencha esse documento por conta própria, ok?
Não deixe de usar nossas dicas de escrita de README de projetos, e deixe sua criatividade brilhar!
:warning: IMPORTANTE: você precisa deixar nítido:
- quais arquivos/pastas foram desenvolvidos por você; 
- quais arquivos/pastas foram desenvolvidos por outra pessoa estudante;
- quais arquivos/pastas foram desenvolvidos pela Trybe.
-->
