# CONTEUDOS-Javascript
Repositorio destinado a resumo com os principais conceitos e principios orientadores de trabalho, com o objetivo de ser utilizado como consulta em situações necessárias do cotidiano.


## INDICE



1. TIPOS PRIMITIVOS
   
       1.1 Tipo Number
 
       1.2 Tipo String
 
       1.3 Tipo Boolean
 
2.  VARIAVEIS
   
3.  FUNÇÕES

4.  Estrutura do `if`



## 1. Tipos Primitivos



É fundamental que o JavaScript consiga determinar qual é o tipo de dado para poder manipulá-lo. Por exemplo, para executar cálculos matemáticos, o dado armazenado na variável precisa ser um número.

### 1.1 Tipo Number


```
// tipo Number

const meuNumero = 3;

const primeiroNumero = 1;
const segundoNumero = 2;

const operacaoMatematica = primeiroNumero + segundoNumero;

console.log(operacaoMatematica)
```


Operadores  `+`, `-`, `/`, `*`

Podemos operar com números negativos, positivos e assim por diante. Normalmente, em linguagem de programação, não estamos restritos a números inteiros, mas podemos trabalhar com números que costumamos chamar de decimais em nosso cotidiano, que têm um ponto seguido de outros números.


### Ponto Flutuante no JavaScript



No JavaScript, podem ser declarados da mesma forma que declaramos os números inteiros e, na hora de associar um valor a ele, podemos apenas inserir o ponto seguido pelo valor desejado.

Então, por exemplo, colocamos 3.3 em uma constante chamada numeroPontoFlutuante.


```
// código omitido

// ponto flutuante

const numeroPontoFlutuante = 3.3;
```

Por exemplo, 0.5, nós podemos declará-la apenas como .5.

`0.30303030303030304` - Existe muitos dígitos após a vírgula e desejamos truncar apenas para dois, por exemplo. O JavaScript tem várias ferramentas prontas de operações matemáticas das mais simples até as um pouco mais complexas.


### Not a number no JavasScript



Acontece Quando o JavaScript tenta fazer operações com números, mas ele não consegue. 

Principalmente quando tentamos multiplicar duas coisas e alguma delas ou as duas não são realmente um número. Nesse caso, em vez de retornar um erro, o JavaScript retorna NaN(NOT A NUMBER).


**Dica: podemos utilizar o número PI através do código Math.PI.**


↪️
[Como formatar número com JavaScript](https://www.alura.com.br/artigos/formatando-numeros-no-javascript?_gl=1*1j0vrgf*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwOTczMTQ4NS4zNS4xLjE3MDk3MzM0NTAuMC4wLjA.*_fplc*UEg3RkVXQTFWQXpOU3BGdUdoWkpOWDR6Qmk2QkJFbmR4RXpEdjl1OVh6Qm1DZCUyRnRwVDJ3UzZ4UDZja0NwWjVJWEhta3JaUUZuanZHcDRXa3UwUXNOJTJCeGtsME5Ca0g0dWszU1pFRFIlMkJITVU0MHNFZ2VGR3E1JTJCanlkZU5nYXclM0QlM0Q.)


↪️
[Como ordenar uma sequência de números no JavaScript](https://www.alura.com.br/artigos/ordenacao-de-numeros-no-javascript-nao-funciona?_gl=1*164k246*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwOTczMTQ4NS4zNS4xLjE3MDk3MzM0NzkuMC4wLjA.*_fplc*UEg3RkVXQTFWQXpOU3BGdUdoWkpOWDR6Qmk2QkJFbmR4RXpEdjl1OVh6Qm1DZCUyRnRwVDJ3UzZ4UDZja0NwWjVJWEhta3JaUUZuanZHcDRXa3UwUXNOJTJCeGtsME5Ca0g0dWszU1pFRFIlMkJITVU0MHNFZ2VGR3E1JTJCanlkZU5nYXclM0QlM0Q.)


###  1.2 Tipo String



tipos textuais, que não se enquadram na categoria de números ou booleanos.

Podemos utilizar para armazenar texto, caracteres, como, por exemplo, letras do alfabeto, pontuação e, basicamente, qualquer coisa que quisermos.

Para criar uma string em JavaScript, precisamos usar aspas, podendo ser duplas ou simples. Tudo que colocarmos entre aspas, o JavaScript considerará como uma string. Isso pode também incluir apenas números.


```
type-string.js

const texto1 = "Olá, mundo!";
const texto2 = 'Olá, mundo!';
const senha = "senhaSuperSegura456!";
```


Ao citar algo que alguém disse em um texto, podemos iniciar com aspas simples, inserir o texto da citação e destacar a citação com aspas duplas.


```
type-string.js

const texto1 = "Olá, mundo!";
const texto2 = 'Olá, mundo!';
const senha = "senhaSuperSegura456!";
const StringDeNumeros = "34567";

const citacao = 'O Leo disse "oi!"'
```


Além disso, temos *outro tipo de aspa, que na verdade é um acento grave*, que conseguimos utilizar também como se fossem as aspas da string. Isso se chama `template string`  ou `template literal`.


**Strings em variáveis**  - `concatenação`



![image](https://github.com/FlavianaFXT/Javascript-Tipos-variaveis-e-funcoes/assets/113718720/609f05fc-ad7d-400a-a7a8-897e23b69562)


**Codificação de strings**



Nas últimas décadas, foram desenvolvidos diversos conjuntos de caracteres especiais, cada um com seus próprios códigos, para que pessoas que escrevem e leem em linguagens diferentes do inglês pudessem utilizar computadores com seus próprios idiomas. 

Para que o computador consiga decifrar um caractere especial, é preciso utilizar um sistema específico que tenha basicamente um código para cada caractere, e que o computador possa acessá-lo para fazer a conversão - uma ideia similar a que está por trás da criptografia.

Foram desenvolvidos diversos conjuntos de caracteres, desde os específicos de cada linguagem como Western, Latin-US, Japanese e assim por diante, até o ASCII (American Standard Code for Information Interchange ou ”Código Padrão Americano para o Intercâmbio de Informação”) e a partir de 2007 foi adotado o formato Unicode. O padrão UTF (de Unicode Transformation Format ou “formato de conversão de unicode”, em tradução livre) é utilizado como padrão na web até hoje.

O Unicode tem códigos específicos para “cifrar” e “decifrar” caracteres de mais de 150 idiomas antigos e modernos, e também diversos outros conjuntos de caracteres como símbolos matemáticos e inclusive emojs. A [Wikipedia](https://en.wikipedia.org/wiki/List_of_Unicode_characters) tem uma lista extensa de todas as tabelas com os códigos Unicode e os caracteres, como por exemplo os que estão abaixo:

caractere	UTF-16	descrição oficial
$	U+0024	DOLLAR SIGN
A	U+0041	LATIN CAPITAL LETTER A
✅	U+2705	CHECK MARK
ぁ	U+3041	HIRAGANA LETTER SMALL A
Podemos testar a transformação/conversão do código Unicode em caractere utilizando o console.log(). Faça o teste:


```
const cifrao = '\u0024'
const aMaiusculo = '\u0041'
const tique = '\u2705'
const hiragana = '\u3041'

console.log(cifrao)
console.log(aMaiusculo)
console.log(tique)
console.log(hiragana)
```


Os caracteres \u no início do código são caracteres de escape que usamos para sinalizar ao JavaScript de que estamos falando de códigos Unicode, e não de strings de texto usuais.

O JavaScript usa, por padrão, o UTF-16. O número 16 está relacionado aos espaços em bits ocupados por cada caractere, 16 neste caso. Não vamos nos aprofundar na relação entre tipos de dados e espaço de memória ocupado por cada tipo - você pode pesquisar mais sobre o assunto, assim como sobre o que são caracteres de escape! - mas por enquanto é bacana vermos na prática como o Unicode funciona.

Bancos de dados podem aceitar outros tipos de codificação de caracteres, o que faz sentido se pensarmos que o UTF-16 utiliza uma quantidade relativamente grande de espaço em memória para salvar cada caractere. 16 bits parece pouco, mas algumas vezes os bancos precisam salvar quantidades enormes de dados! Porém, com as tecnologias de armazenamento e tráfego de dados que temos hoje, esta já não é uma preocupação tão grande, a não ser em casos muito específicos. Já não é muito comum utilizar uma codificação diferente da UTF em bancos mesmo em caso de grandes volumes de dados, mas sempre vai depender muito do caso.

Mais detalhes precisos e documentação sobre o Unicode na página da [Unicode Foundation](https://home.unicode.org/).


## Métodos e ferramentas prontas do Javascript




| O que | Como | Sobre |
| --- | --- | --- |
| para transformar todas as letras em minúsculo | `.toLowerCase()` | [MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase). |
| para transformar tudo em maiúsculo | | |
| para contar quantas letras tem uma cadeia de caracteres | `.length`| [aqui](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase) |
| para retirar espaços | | |


[métodos de string do MDN (são vários)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String#m%C3%A9todos), com a descrição de cada um.


### 1.3 Tipo Boolean



`tipo booleano` - também conhecido como verdadeiro e falso, ou true ou false.

É peculiar, pois não é um número nem um texto e possui apenas dois valores: podemos ter somente true ou false.

Usamos os booleanos com frequência quando precisamos fazer alguma comparação, como, por exemplo, em estrutura if-else, estrutura while e estrutura for.

**OBS**: Quando se utiliza apenas um sinal de igual no JavaScript, ocorre uma atribuição de valor a uma variável. Portanto, o valor à direita do sinal de igual é atribuído à variável mencionada à esquerda.

Para comparações no JavaScript,usamos dois ou três sinais de igual e o resultado das comparações sempre será Verdadeiro ou falso.


```
type-boolean.js

const primeiroNumero = 5;
const segundoNumero = 5;

console.log(primeiroNumero === segundoNumero);
```


**Boolean como valores de variáveis**



Além de comparação, ele pode assumir valores de variáveis. Então, por exemplo, a variável `cadastroAtivo`, pode inicialmente ter valor falso. E podemos executar alguns testes, como verificar a senha, e ele assumir um novo valor de verdadeiro, significando que o cadastro está ativo.


```
type-boolean.js

// boolean
// true -> verdadeiro
// false -> falso

const primeiroNumero = 5;
const segundoNumero = 5;
let cadastroAtivado = true;

console.log(primeiroNumero === segundoNumero);
```


**Comparando duas strings com boolean**




```
type-boolean.js

// boolean
// true -> verdadeiro
// false -> falso

const primeiroNumero = 5;
const segundoNumero = 5;
let cadastroAtivado = true;

//console.log(primeiroNumero === segundoNumero);

const texto1 = "Alura";
const texto2 = "alura";

console.log(texto1 === texto2)
```


2. VARIAVEIS




*VARIAVEIS* Quando um programa precisa armazenar um valor para usar futuramente, já sabemos que usamos variáveis para isso.


## Var, Let e Const



`var` --> funciona basicamente em qq parte do codigo
`let` --> surgiu com o js 2015
`const` --> impede que alguem mude o valor da variavel;


### Tipos null e undefined



O `null` é um tipo especial, pois pode ser traduzido como “ausência de valor” e pode ser atribuído como valor de uma variável:


```
let input = null;

if (input === null) {
 console.log('não há informação');
} else {
 console.log(input);
}

Nesse caso, qual seria a diferença entre os dois casos abaixo?

let input = null;
let input2;

console.log(input); // null
console.log(input2); // undefined
```

`undefined`. Este tipo também representa “ausência de valor”, porém de uma outra forma: usualmente, enquanto null é um valor atribuído a uma variável que existe e foi iniciada, undefined se refere ao valor de uma variável que não foi inicializada (ou seja, não foi atribuído nenhum valor a ela).

undefined também é o valor retornado por uma função que não tem cláusula return.

embora os dois tipos sejam utilizados para sinalizar ausência de valor, os operadores de comparação do JavaScript podem ou não diferenciá-los:


```
console.log(null == undefined); // true
console.log(null === undefined); // false
```


No cotidiano é comum considerar undefined como uma ausência de valor “inesperada” (causada por um bug ou erro no código) e null como um tipo de dado que também significa ausência de valor, mas não de maneira inesperada. Por exemplo, um campo em uma tabela de um banco de dados que esteja sem dados ou uma informação solicitada que não seja obrigatória e não tenha sido preenchida pelo usuário pode ter valor null.


## Padrão de nomes no JavaScript



cada linguagem possui seus próprios padrões. 

A primeira coisa que precisamos ter em mente é que o JavaScript é case-sensitive, ou seja, diferencia maiúsculas e minúsculas. 


```
const minhaVar = 1;
const MinhaVar = "texto";
const minhavar = "3";
const MINHAVAR = 2;

console.log(minhaVar, MinhaVar, minhavar, MINHAVAR)
```


convenções - boas práticas e padronização, para padronizar estes aspectos do código.

Existem várias convenções para nomes e cada linguagem de programação tem o seu. Seguem alguns deles:


```
camelCase: Inicia com letra minúscula e a primeira letra de cada palavra em seguida é escrita com letra maiúscula. Por exemplo: minhaVar ou senhaDoUsuario. Esta é a convenção utilizada pelo JavaScript para variáveis e funções.
snake_case: Os espaços são substituídos pelo caractere _ (underline), com todas as palavras em letra minúscula. Por exemplo: minha_variavel ou senha_do_usuario.
kebab-case: Similar ao anterior, porém com os espaços substituídos por hífens. Por exemplo: minha-var ou senha-do-usuario. Esta convenção não pode ser utilizada no JavaScript para variáveis e funções.
PascalCase: Similar ao CamelCase, porém neste caso todas as palavras começam com letra maiúscula. Por exemplo: MinhaVar ou SenhaDoCliente.
Importante: Nunca utilize espaço nem caracteres especiais, nem inicie os nomes das variáveis com números.
```


Se você utilizar qualquer um dos padrões acima para nomear variáveis com JavaScript (com exceção do padrão kebab-case), seu código continuará funcionando, mas seguir as convenções é parte de desenvolver um código legível e bem escrito.


## 3. FUNÇÕES



A maneira mais clássica de escrever uma função em JavaScript e em várias outras linguagens de programação é começar com a palavra function, seguida do nome da função e de parâmetros opcionais. Dentro da função, um bloco de código descreve a ação que a função deve realizar.

Quando desejamos executar a função, a chamamos pelo nome e passamos o parâmetro necessário a ela. Este parâmetro pode ser uma string, outra função, um texto, um número, entre outros.


```
function minhaFuncao(param) {
  // bloco de código
}

minhaFuncao("param")
```


No entanto, existe outra maneira de escrever funções em JavaScript, que chamamos de `expressão de função`. Na expressão de função, a função não tem um nome; criamos uma variável, neste caso criada com const, e atribuímos nossa função a essa variável.


```
const soma = function(num1, num2) {return num1 + num2}
console.log(soma(1, 1))
```


**OBS**: antes de executar qualquer coisa no código, o JavaScript lista as funções declaradas e o que foi declarado como var. Antes de iniciar qualquer atividade, o JavaScript já sabe o que é. Por isso, funciona chamar a função declarada antes dela "existir" no código.


`Arrow Function`

A arrow function é uma função de seta, isso porque utiliza uma seta na sua sintaxe. Essa é uma novidade do ES6. é semelhante à expressão de função. 


```
function apresentar (nome) { 
return meu nome é ${nome}`; 
}

const apresentaArrow = nome => `meu nome é ${nome}`;
```


 A Arrow Function foi introduzida junto com o ES6, em 2015, e deixou o código muito menor, pois agora podemos declarar tudo em uma única linha, não precisamos de chaves, nem retornar nada.

Além disso, ela não pode ser nomeada, ou seja, essa opção não está nem disponível e também sempre precede uma constante com o nome da variável que será utilizada.  Se o código tiver mais de uma linha de instrução será preciso usar as chaves e o return.

A arrow function é uma forma rápida e concisa de escrever funções, tornando o código mais limpo.

A arrow function também possui vantagens quando estamos trabalhando com objetos.


## 4. Estrutura do `if`



As estruturas condicionais são essenciais para a programação, pois permitem que um programa execute este ou aquele bloco de código de acordo com uma condição, por exemplo: “Se o e-mail e a senha estiverem corretos, o usuário poderá acessar o sistema. Senão ele deve receber um aviso de credenciais de acesso incorretas”. Uma condição exclui automaticamente a outra, pois ou ambas as credenciais (e-mail e senha) estarão corretas, ou não.

As estruturas condicionais permitem que o código se ramifique e tome “caminhos” diferentes de acordo com a condição fornecida.

Abaixo, vamos relembrar a estrutura condicional if e suas variações:

A principal estrutura condicional é if, que podemos traduzir literalmente como “se”:


```
if (condicao) {
 // código a ser executado
}
```


A condicao é sempre uma expressão que deverá ser avaliada e retornar true ou false (ou seus equivalentes “truthy” ou “falsy”). O bloco de código dentro do if só será executado caso a expressão retorne true ou um valor “truthy”.


**Múltiplas condições**



É possível usar os operadores AND (&&) ou OR (||) para executar o código no if caso uma das condições for verdadeira, ou as duas:


```
const num = 11;

if (num > 10 || !num) {
 console.log('número não válido');
}
```


Também é possível usar o operador lógico && (and ou e em português) para especificar que a condição do if será validada apenas se todas as condições retornarem true:


```
const num = 11;

if (num > 10 && num < 20) {
 console.log('número válido');
}
```


**if…else**



Outra forma de condicional muito utilizada é adicionar a cláusula else para ser executada quando a condição do if retorna false. Podemos ler if…else como “se… senão”, como por exemplo “se uma dada condição for verdadeira (true) execute um determinado código; senão, execute outro código”.


```
function verificaNumero(numero) {
    if (numero > 10) {
         return 'número maior que 10';
    } else {
        return 'número não é maior que 10';
    }
}

console.log(verificaNumero(9)) //número não é maior que 10
```


**else if**



A condicional if…else vai executar um bloco de código entre duas possibilidades, dependendo do resultado da expressão que é passada como condição do if. Porém, em alguns casos é necessário mais de duas opções de fluxo para o código; para estes casos existe a cláusula else if:


```
const num = 15;

if (num >= 0 && num <= 10) {
  console.log('número entre zero e dez');
} else if (num > 10 && num <= 20) {
  console.log('número entre dez e vinte');
} else if (num > 20 && num <= 30) {
  console.log('número entre vinte e trinta');
} else {
  console.log('outro número');
}
```


** IMPORTANTE: Ao trabalhar com múltiplas condições e else if, lembre-se sempre que cada condição e cada bloco (if, else if e else) deve representar condições excludentes entre si! Ou seja, não pode haver ambiguidade entre as condições - uma mesma condição válida tanto no if quanto no else if, por exemplo. **




