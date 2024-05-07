# CONTEUDOS-Javascript
Repositorio destinado a resumo com os principais conceitos e principios orientadores de trabalho, com o objetivo de ser utilizado como consulta em situações necessárias do cotidiano.


## INDICE


- [1 TIPOS PRIMITIVOS](#1-TIPOS-PRIMITIVOS)
   - [ 1.1 Tipo Number](#1.1-Tipo-Number)
     - [Ponto Flutuante no JavaScript](#Ponto-Flutuante-no-JavaScript)
   - [ 1.2 Tipo String](#1.2-Tipo-String)
   - [ 1.3 Tipo Boolean](#1.3-0Tipo-Boolean)
- [2 VARIAVEIS](#2-VARIAVEIS)
- [3 FUNÇÕES](#3-FUNÇÕES)
- [4 ESTRUTURA DO `if`](#4-ESTRUTURA-DO-`if`)
- [5 ARRAYS](#5-ARRAYS)
   - [5.1 Introdução a Arrays](#5.1-Introdução-a-Arrays)
     - [Adicionando Elementos](#Adicionando-Elementos)
     - [Deletando Elementos](#Deletando-Elementos)
   - [5.2 Metodos de Array](#5.2-Metodos-de-Array)
   - [5.3 Alterando Arrays](#5.3-Alterando-Arrays)
     - [Dividindo com slice()](#Dividindo-com-slice())
     - [Alterando com splice()](#Alterando-com-splice())
     - [Alterando Strings com map()](#Alterando-Strings-com-map())
   - [5.4 Concatenando Arrays](#5.4-Concatenando-Arrays)
      - [Lista com 2 Dimensões](#Lista-com-2-Dimensões)
      - [Matrizes](#Matrizes)
   - [5.5 Laços de Repetição](#5.5-Laços-de-Repetição)
     - [Desestruturando uma lista](#Desestruturando-uma-lista)
     - [For Clássico](#For-Clássico)
     - [Loop infinito](#Loop-infinito)
     - [Média com FOR](#Média-com-FOR)
     - [Loops em matrizes](#Loops-em-matrizes)
     - [Media com FOR OF](#Media-com-FOR-OF)
     - [Possibilidades do for](#Possibilidades-do-for)
- [6 FUNÇÕES CALLBACK](#6-FUNÇÕES-CALLBACK)
      - [Média com FOR EACH](#Média-com-FOR-EACH)
     - [for...of vs callbacks](#for...of-vs-callbacks)
     - [forEach()](#forEach())
     - [Método map()](#Método-map())
     - [map() e forEach](#map()-e-forEach)
 - [7 AVANÇANDO EM ARRAYS](#7-AVANÇANDO-EM-ARRAYS)
   - [7.1 Filtrando Elementos](#7.1-Filtrando-Elementos)
     - [Retorno do filter](#Retorno-do-filter)
   - [7.2 Somando com Reduce](#7.2-Somando-com-Reduce)
     - [estrutura do reduce()](#estrutura-do-reduce())
   - [7.3 Clonando com spread operator](#7.3-Clonando-com-spread-operator)
   - [7.4 Removendo Elementos Repetidos](#7.4-Removendo-Elementos-Repetidos)
      - [estrutura Set](#estrutura-Set)
     
   

       
## 1 TIPOS PRIMITIVOS



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


#### **Comparando duas strings com boolean**



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


## 2 VARIAVEIS


*VARIAVEIS* Quando um programa precisa armazenar um valor para usar futuramente, já sabemos que usamos variáveis para isso.


## 2.1 Var, Let e Const



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


### Padrão de nomes no JavaScript



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


## 3 FUNÇÕES



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

Para saber mais sobre arrow functions leia o artigo - [Conhecendo Arrow Functions](https://www.alura.com.br/artigos/conhecendo-arrow-functions?_gl=1*1gij91k*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwNTMzODQ1OC4xNi4xLjE3MDUzMzg5MzQuMC4wLjA.*_fplc*dW9uU0VaVkprRURiWDduU043TzUwWE4zNllKUFczMG4lMkJyM2FsMVdJUW1sNzhVbENibDZ0VFRYUGtFdG1ZR29COHdXNG5CYURnQTJKMUtnZVRuaU56TElPbldVakxyMHp5MzE3MW9uY2YxNGZEUEx2cHMlMkJGaWtqZWlJZXRKZyUzRCUzRA..) no site da Alura. 



## 4 Estrutura do `if`



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


### 4.1 **Múltiplas condições**



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



**Poderíamos usar um loop para percorrer todas as letras de um string?**


“String”, além de ser o tipo de dado usado para representar textos, também se define como uma sequência ordenada de caracteres!

“Lista ordenada” (ou sequência) também é uma forma de definir arrays, certo? Então podemos pensar que, por baixo dos panos, strings são armazenadas em memória da seguinte forma:


```bash
const nome = "Alura";
// ["A", "l", "u", "r", "a"]
```


Ou seja, é possível utilizar alguns métodos de array e laços de repetição para acessar e alterar strings:


```bash
const nome = "Alura";
let nomeMaiusculas = "";

for (let i = 0; i < nome.length; i++) {
 nomeMaiusculas += nome[i].toUpperCase()
}
console.log(nomeMaiusculas) //ALURACOPIAR CÓDIGO
const nomedoCurso = "Fundamentos de JS";
const nomeDaPlataforma = " Alura"

const nomeCompleto = nomedoCurso.concat(nomeDaPlataforma)
console.log(nomeCompleto)  //Fundamentos de JS Alura
```


Você pode conferir a lista completa de métodos de string na - [documentação do MDN]( https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String#methods) .


### 4.2 **if…else**



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


### 4.3 **else if**



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


## 5 ARRAYS

é um tipo de estrutura de dados. Ao contrário de uma variável, que guarda somente um valor por vez, um array (ou lista) pode armazenar diversos valores. Pode ser usada, por exemplo, para agrupar diversos dados que têm relação entre si.

```bash
const numero1 = 50;
const numero2 = 43;
const numero3 = 12;
```


```bash
// utilizando array
const numeros = [50, 43, 12];
```

Um array pode ser definido como uma lista ordenada de valores enumerados em que cada valor é chamado de elemento ou item, e cada elemento se localiza numa posição na lista chamada de índice. Ou seja, uma lista ordenada de valores enumerados. Quando falamos de valores, estamos nos referindo a dados de algum tipo: string (texto), number (número), booleano (true ou false) ou outros dados reconhecidos pelo JavaScript.

Quando trabalhamos com arrays, chamamos de elemento ou item cada um dos valores da lista.

Lembrando que cada elemento corresponde a um dado, separados por vírgula.



### 5.1 Introdução a Arrays


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/fa089fef-beb9-4afb-8d4d-d222d50764ef)


### **Como funcionam os arrays**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/ba1a8335-ca1b-495c-b9d6-869e4def9f92)


Toda lista precisa de um identificador — no caso, temos notas.

Cada um dos valores de um array está guardado dentro de uma "caixinha", que representa um espaço na memória que o nosso computador reservou para armazenar esse valor. Então, temos uma caixinha com o valor 10, outra caixinha com valor 6.5, outra com valor 8 e outra com valor 7.5.

Vale lembrar que um array pode ter o tamanho que nós quisermos.

Cada um dos valores de um array pode ser chamado de elemento, item ou valor.

cada um desses itens tem um identificador numérico único. Esses identificadores são chamados de índices ou posições. Eles sempre começam no zero e aumentam de um em um, até onde for necessário.

Se um array é uma lista ordenada, então é possível acessar cada um dos dados (ou valores) nele se soubermos a posição dele na lista. Por exemplo:


```bash
const nums = [50, 43, 12];
// o número 43 está na posição de número 1 (segunda posição) nessa lista de três números.
```

A `propriedade length`:  especifica o tamanho de um array, ou melhor dizendo, o número de elementos. É importante notar que não estamos falando aqui de índices ou posições, e sim da quantidade de valores (dados) contidos no array. Por exemplo:


```bash
// índice     0   1   2   3
const nums = [50, 43, 12, 98];
console.log(nums.length) //
```


Considerando que o array acima tem 4 elementos, podemos dizer que o valor retornado por length sempre será 1 número a mais do que o valor de índice mais alto. Neste caso, o array nums é um array de 4 elementos e seus índices vão de 0 a 3.


*Listas e tipos de valor*

vale ressaltar que as listas do JavaScript não se restringem a um único tipo de dado. Em um único array, podemos ter o valor 10 , uma string "oi" e um valor true e outro false (booleanos). É possível colocar todos esses valores em uma mesma lista, apesar de não ser comum. Considera-se uma boa prática trabalhar com o mesmo tipo de dado em um array, mas o JavaScript permite inserir diferentes tipos de dados em um mesmo array.


#### **Adicionando Elementos**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/3234d56e-1541-4b56-b340-f2b8819f8070)


*Desafio 2: Adicionando elementos*

Um professor acidentalmente passou apenas 3 das 4 notas no sistema para um aluno:

10
6
8

Para corrigir, precisamos adicionar a nota 7 e fazer o cálculo da média corretamente.

*Alterando constantes?*

Por mais que declaremos um array como constante, conseguimos alterá-lo de acordo com alguns métodos do próprio array. Quando criamos uma constante no JavaScript, somos somente impedidos de fazer uma nova atribuição para a constante.


#### **Deletando Elementos**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/c57fe0ad-37d7-4f0f-9c24-0626efd0b8ce)


*Desafio 3: Deletando elementos*

Dessa vez, um dos professores acidentalmente lançou 5 notas no sistema para um aluno:

```
10
6
8
5.5
10
```


Para corrigir, precisamos que remover a última nota e fazer o cálculo da média corretamente.

Para remover a última nota, usaremos outro `método dos arrays` do JavaScript — o `pop()`.


## 5.2 Metodos de Array


Um método é uma função que serve como uma propriedade do array ou de um objeto (que veremos em outro curso). Ele pode realizar tarefas pré-definidas usando os dados do array e dos parâmetros que passamos para eles, como adicionar, remover ou até encontrar elementos.

Os principais são:


| METODO | DESCRIÇÃO |
| --- | --- |
| `concat()` | Junta dois arrays, colocando o array passado como argumento, logo depois do primeiro. Em português essa operação é conhecida como concatenação. Não altera o array no qual foi chamado, então precisamos salvar esse resultado em um novo array. |
|  `filter()`  |  Retorna uma lista contando todos os elementos que passaram em um teste, ou seja, uma função escrita por nós. Não altera o array onde foi chamado, então precisamos salvar esse resultado em um novo array. |
|  `find()` |  Funciona de forma parecida com o filter, porém retorna apenas o primeiro valor que satisfizer o teste, podendo ser uma string ou um número. |
| `findIndex()` | Funciona igual o find(), mas retorna o índice em vez do elemento, possibilitando usá-lo em outras partes do código.  |
| `lastIndexOf()` |  É igual o findIndex() porém começa do último elemento, não no primeiro. |
|  `forEach()`  | Executa uma função em cada elemento do array de forma individual. Não altera o array original e nem retorna um valor, deixando esse trabalho a cargo da função escolhida.   |
|  `pop()`  |  Retira o último elemento do array. Altera o array original removendo o elemento.  |
|  `shift()`  |  Retira o primeiro elemento do array. Altera o array original removendo o elemento e trocando o índice de todos os elementos para um a menos do que eram, o índice 1 passa a ser o 0, o 2 passa a ser o 1, e assim por diante.  |
|  `push()` |   Adiciona o elemento passado como parâmetro do array, porém na última posição. Altera o array original com o novo valor.  |
| `unshift()`  |  Funciona igual ao push(), porém adiciona na primeira posição e acaba trocando o índice de todos os elementos. Altera o array original com o novo valor. |
| `reduce()` |  Utiliza uma função definida pelo usuário em cada um dos elementos, guardando o resultado em uma variável que pode ser acessada dentro da função que foi definida, retornando um único valor no final, reduzindo o array para um único valor. |
| `reduceRight()` |  Funciona igual o reduce() porém começa do final do array e segue até o início. |
| `reverse()`  |   Inverte a ordem dos elementos do array, então o primeiro vira o último, o segundo o penúltimo e assim por diante. |
| `slice()`  |  Copia uma parte do array para outro array. |
| `sort()` |  Organiza o array de acordo com a classificação Unicode, onde os números vêm antes das letras, porém não funciona corretamente para números, onde temos que definir uma função que irá auxiliar o comando. |
| `splice()` |  Consegue remover, um ou mais elementos consecutivos caso o segundo parâmetro tenha um valor maior que 0, e incluir um ou mais elementos a partir de um índice escolhido. |
| `includes()`  |  confere se o elemento passado por parâmetro está incluso em uma lista; |
| `indexOf()`  | retorna o índice do elemento passado por parâmetro.  |
|   |   |



Em caso de dúvidas sobre como funciona um método de array, você sempre pode consultá-lo na - [documentação oficial da MDN]( https://developer.mozilla.org/pt-BR/)

podemos consultar rapidamente o que o método faz, seu valor de retorno e se ele altera o array original.

A documentação também fornece informações bastante detalhadas sobre cada recurso da linguagem; você não precisa entender tudo que é mencionado em cada página (e no início de desenvolvimento, você provavelmente irá se deparar com muitos termos novos), mas ela é uma excelente fonte de consultas. Além disso, ela fornece vários exemplos práticos onde um método pode ser útil. A documentação será muito importante na sua jornada de desenvolvimento!



## 5.3 Alterando Arrays


#### **Dividindo com slice()**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/aeb6b29e-b5c7-4882-a06b-5f031d504a47)


*Desafio 4: Sala dividida*

Temos uma sala de aula com 20 estudantes, representados por uma lista de strings:

'João', 'Juliana', 'Ana', 'Caio', 'Lara', 'Marjorie', 'Guilherme', 'Aline', 'Fabiana', 'Andre', 'Carlos', 'Paulo', 'Bia', 'Vivian', 'Isabela', 'Vinícius', 'Renan', 'Renata', 'Daisy', 'Camilo'

Nosso desafio é dividi-los em duas salas com a mesma quantidade de pessoas. Isto é, duas listas com 10 estudantes, cada.

Informaremos dois parâmetro para o método slice(), separados por vírgula. O primeiro indicará a posição do elemento em que começaremos a "fatiar" a lista original. No caso, começaremos por João, que está na posição 0. O segundo parâmetro indicará onde terminaremos de "fatiar". No caso, colocaremos o valor 10, que se refere ao índice do 11° estudante, André.

Existe uma peculiaridade do método slice() que devemos nos atentar! No segundo parâmetro, informamos o índice de um elemento e esse elemento não será incluído no novo array! Ou seja, ao colocar os parâmetro 0 e 10, estamos selecionando os alunos do índice 0 ao 9.


*Melhorias*

Atualmente, nosso código funciona para uma lista de 20 estudantes. Mas e se tivéssemos uma lista de 30, 40 ou 100 alunos? É interessante que o nosso código seja o mais dinâmico possível. Em vez de escrever valores estáticos (como o 10, que sabemos que é a metade da lista), podemos inserir valores dinâmicos.

Para encontrar a metade do nosso array, em lugar de 10, vamos colocar o tamanho da lista dividido por 2. Faremos isso tanto na atribuição da constante sala1 como em sala2.

 - [documentação do JavaScript](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript)



#### **Alterando com splice()**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/d243d406-2efb-4a45-89fc-f075a1d723f7)


Em inglês, o termo splice significa "emendar" ou "juntar". Cuidado para não confundi-lo com o método slice() que abordamos na última aula, já que seus nomes são parecidos. Até o funcionamento deles é semelhante e pode causar confusão!

O primeiro parâmetro do método splice() é o índice do elemento que queremos remover. Portanto, para remover o nome de Ana, passamos o índice 1. 
O segundo parâmetro é a quantidade de itens que queremos remover a partir desse índice. Logo, para remover o nome de Ana e de Caio, informaremos o valor 2.
O método splice() aceita um terceiro parâmetro. Então, vamos colocar a string "Rodrigo".


#### **Alterando Strings com map()**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/07aa89a6-f45d-4ba1-ae27-0492b1d3f1be)


Precisamos padronizar a lista de alunos para conter apenas letras maiúsculas.


`
ana Julia
Caio vinicius
BIA silva
`


Temos uma lista de strings em que os nomes não estão padronizados, alguns nomes estão com maiúsculas e outros estão com minúsculas. Vamos padronizar para ter maior consistência nos nossos dados.

Como pegar uma string e deixar todas as letras maiúsculas? Usaremos o método toUpperCase(). Mas para utilizar esse método em cada uma das strings da lista, precisamos percorrer o array inteiro, por isso usaremos o map().

Para finalizar, uma particularidade das arrow functions é que quando tudo o que fazemos dentro da arrow function é retornar um valor, podemos simplesmente omitir a palavra-chave return, vamos apagá-la, e podemos tirar as chaves de abertura e chave de fechamento da função. Então tudo o que ficou como callback foi `(nome) => nome.toUpperCase());`.


```bash
const nomes = ["ana Julia", "Caio vinicius", "BIA silva"];

const nomesPadronizados = nomes.map((nome) => nome.toUpperCase());

console.log(nomesPadronizados);
```



## 5.4 **Concatenando Arrays**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/aa7a5c1e-94d4-4006-8e23-b148662390ed)


Mais uma vez, teremos um método para nos auxiliar na junção dessas listas: o concat(), que vem da palavra "concatenar". Em programação, isso significa "juntar".
Dentro dos parênteses desse método, passaremos como parâmetro outra lista. No caso, salaPython.

O método concat() não alterará nenhum dos arrays, ele retornará uma nova lista. Sabendo disso, vamos guardar o resultado numa constante chamada salasUnificadas.
Como resultado, temos um novo array com todos os nomes — primeiro com estudantes de JavaScript e, depois, os de Python. 

Vale lembrar que a ordem em que informamos os arrays afeta a ordem em que os nomes aparecerão na lista final. Para demonstrar essa diferença, vamos inverter as referências na linha em que atribuímos o valor da constante salasUnificadas. Em vez de salaJS, colocaremos salaPython e, em lugar de salaPython, usaremos salaJS.


#### **Lista com 2 Dimensões**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/1fff1b43-ab46-4069-bba8-44e5f25379dd)


*Desafio 7: Lista com 2 dimensões*

Foram fornecidas duas listas para nós. A primeira contém os nomes de quatro estudantes e a segunda possui suas respectivas médias:

'João', 'Juliana', 'Caio', 'Ana'
10, 8, 7.5, 9

Nosso objetivo é criar uma lista que contenha essas duas listas. Já adiantando: é possível uma lista conter outras listas. A seguir, vamos aprender como lidar com esse tipo de dado mais complexo.


*Listas dentro de listas*

No VS Code, vamos criar um arquivo chamado lista-duas-dimensoes.js. Começaremos declarando duas listas, uma com os nomes das pessoas estudantes e outra com suas notas:

Em seguida, vamos declarar uma lista chamada listaDeAlunosEMedias, que conterá as listas alunos e medias. O primeiro elemento será a lista de estudantes e o segundo será a lista de médias:

O retorno pode parecer um pouco estranho, mas está correto. Trata-se de uma lista cujo conteúdo são duas listas. Nas extremidades, abrimos e fechamos os colchetes do array "externo". Dentro dele, temos a lista de estudantes na primeira posição e a lista de médias na segunda posição.


*Acessando elementos*

Conseguimos criar uma lista que contém outras duas listas, mas como faremos para acessar elementos dentro delas? Por exemplo, como podemos selecionar Juliana, que está na posição 1 da lista alunos? Vamos descobrir, a seguir.


bash```

    console.log(
    `A aluna da posição 1 da lista de alunos é: ${listaDeAlunosEMedias[0]}.`
    );
```


```
Portanto, listadeAlunosEMedias[0] representa a lista de alunos. Na sequência, vamos acessar a posição 1 da lista de alunos, pois sabemos que é onde está Juliana. Após [0], basta abrir e fechar outros colchetes e inserir o valor 1 entre eles:


```bash

     console.log(
    `A aluna da posição 1 da lista de alunos é: ${listaDeAlunosEMedias[0][1]}.`
     );
```



Digamos que agora também precisamos indicar a média da Juliana.
Uma vez dentro da lista de médias, vamos acessar a nota de Juliana, que está na posição 1 também. 


```bash

    console.log(
    `A aluna da posição 1 da lista de alunos é: ${listaDeAlunosEMedias[0][1]}.
    A nota dessa aluna é ${listaDeAlunosEMedias[1][1]}.
    `
    );
    
 ```


 #### ** Matrizes **

 listas com duas dimensões, ou seja, arrays que contêm arrays, podendo ter um único array ou vários dentro do principal.

```bash
const nomes = ["Ana", "Juliana", "Leonardo"];
const idades = [30, 35, 28];
const faculdade = [false, true, true];

const funcionarios = [nomes, idades, faculdade];
```


O array funcionarios é um array de duas dimensões. Há 3 arrays dentro dele, e para acessar os valores em funcionarios precisamos de 2 colchetes “[ ] [ ]”. O primeiro colchete será usado para escolher qual dos 3 arrays dentro de funcionarios será acessado. podendo ser:


`
0 -> nomes
1 -> idades
2 -> faculdade
`


O segundo colchete será usado para acessar a informação dentro do array escolhido.

Outra forma de chamar os arrays de 2 dimensões é matrizes. Matrizes podem ser visualizadas como uma tabela do Excel, onde cada campo representa um elemento, e precisamos de uma linha e uma coluna para acessar um campo. Então, as linhas são o primeiro colchete e a coluna o segundo colchete.

Arrays têm seu principal uso quando temos uma grande quantidade de informações com propósitos similares, como as notas de um aluno. Matrizes, por sua vez, são utilizadas quando precisamos de vários arrays similares ou com informações ligadas às outras, como as notas de uma classe com vários alunos.

As matrizes não são limitadas a 2 dimensões, podendo ter mais dimensões, de modo que cada dimensão é representada por um colchete. Porém, tome cuidado para não se perder dentro delas, já que se uma matriz passa a ter, por exemplo, 4 ou 5 dimensões, se torna bem difícil saber exatamente o que está sendo acessado e começamos a ter problemas para fazer a manutenção do código.

vamos ver o que acontece se um dos parâmetros for um array com dois elementos, um número e um array:

```bash
const arrayOriginal = [50, 60, 70]
const arrayConcat = arrayOriginal.concat([80, [90, 100]])

console.log(arrayConcat)
console.log(arrayOriginal)
```


O resultado no terminal agora é:


```bash
[ 50, 60, 70, 80, [ 90, 100 ] ]
[ 50, 60, 70 ]
```` 


Vimos anteriormente que, quando recebe um array como parâmetro, concat() vai concatenar apenas os elementos. Porém, este método não extrai os elementos do array de forma recursiva; ou seja, não vai extrair os elementos de arrays que estejam “aninhados”. Dessa forma, 80 foi extraído do array com sucesso, porém 90 e 100 não, o método considerou [90, 100] como um único elemento.

concat() é um método útil quando não se deseja alterar o array original, e sim fazer uma cópia alterada. Caso isso não seja necessário, considere utilizar push() ou splice() para inserir novos elementos ou fazer alterações no array original.



## 5.5 Laços de Repetição


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/2bce8028-6631-4112-af0e-6f3a86cf2e03)


*Desafio 8: Procurando na lista* 


Crie uma função que recebe como argumento o nome de um aluno.
Verifique se o aluno está presente na lista e retorne a média final que se encontra no mesmo índice.
Caso o nome do aluno não esteja na lista, retorne uma mensagem indicando que o aluno não foi encontrado.
Para este desafio, usaremos as mesmas listas da aula anterior:

`
'João', 'Juliana', 'Caio', 'Ana'
10, 8, 7.5, 9
`

*Checando nomes cadastrados*

Vamos criar uma função chamada exibeNomeENota(), que verificará se o nome de uma pessoa está cadastrado na lista e, depois, mostrará sua nota. Essa função receberá como parâmetro o nome do aluno:
Primeiramente, criaremos uma lógica para checar se conseguimos exibir uma mensagem ou não, a depender se o nome está presente ou não na lista.

Em exibeNomeENota(), acessaremos apenas a listaDeAlunosEMedias, para nos acostumarmos com a sintaxe de arrays de duas dimensões. Em cenários reais, nem sempre teremos acesso direto a essas listas "internas" como temos agora, então é importante estar familiarizado com essa sintaxe.

Dentro da função exibeNomeENota(), vamos desenvolver uma estrutura if:

Como condição, avaliaremos se o aluno está na lista ou não. Como a lista de alunos está na posição 0 da listaDeAlunosEMedias, usaremos a sintaxe listaDeAlunosEMedias[0] para nos referir a ela. Em seguida, usaremos o método includes() — que significa "incluir", em inglês. Como parâmetro dele, passaremos aluno:
Vamos incluir o else também. Caso o aluno não seja encontrado, exibiremos outra mensagem explicativa:

O método includes() verifica se o parâmetro passado para ele está incluso na lista. Quando está incluso, o retorno será o valor booleano true (verdadeiro). Do contrário, o retorno será false(falso). Por isso, podemos usar o includes() como condição da estrutura if.

Portanto, já criamos um código para definir se um nome está presente na lista. Vamos continuar complementando o código para sustentar o desafio.


*Exibindo a média*

Conforme o desafio, quando o aluno estiver incluso na lista, temos que procurar sua média e exibi-la. Sabemos que a média está no mesmo índice do aluno, porém em outra lista. Por exemplo, João está no índice 0 da lista alunos e sua média está no índice 0 da lista medias. Então, para descobrirmos a média de um aluno, precisamos saber seu índice.

Para encontrar o índice de um elemento em um array, podemos usar o método indexOf() — que significa "índice de", em inglês. Vamos utilizá-lo dentro do bloco if, após o console.log():

Como o objetivo é pesquisar no array alunos, referenciamos essa lista com listaDeAlunosEMedias[0]. Em seguida, usamos o método IndexOf(), que retornará o índice do aluno passado por parâmetro. Guardamos esse retorno na constante indice.

Sabemos que o índice de João é 0, então nosso código está funcionando e aplicamos o método indexOf() corretamente.

Agora que conseguimos selecionar o índice do aluno, vamos pesquisar sua média! A princípio, declararemos a constante mediaDoAluno. Para referenciar a lista medias, usaremos a sintaxe listaDeAlunosEMedias[1]. Em seguida, acessaremos o elemento no mesmo índice do aluno:


*Refinamentos* 

Por fim, vamos alterar a mensagem exibida no console para torná-la mais objetiva e remover alguns trechos desnecessários do nosso código.

Primeiro, vamos apagar o console.log() em que mostramos a mensagem de que o aluno está cadastrado. E, no console.log() que está dentro do bloco if, vamos utilizar uma template string com uma mensagem mais explicativa.


 ```bash
     function exibeNomeENota(aluno){
         if (listaDeAlunosEMedias[0].includes(aluno)) {
             const indice = listaDeAlunosEMedias[0].indexOf(aluno);
     
             const mediaDoAluno = listaDeAlunosEMedias[1][indice];
     
             console.log(`${aluno} tem a média ${mediaDoAluno}.`);
     
         } else {
             console.log("Aluno não encontrado!");
         }
     }
 
     exibeNomeENota("Juliana");
 ```


#### **Desestruturando uma lista**


*Refatoração*


Tem algo no nosso código que podemos melhorar. Dentro do bloco if, escrevemos listaDeAlunosEMedias[0] para treinar a sintaxe de listas de duas dimensões. Porém, não fica intuitivo o que essa expressão significa, não fica claro que a posição 0 de listaDeAlunosEMedias se refere à lista de alunos. Vale lembrar que também estamos simulando um cenário em que apenas temos acesso à listaDeAlunosEMedias (e não diretamente à lista alunos).

Antes da constante indice, podemos declarar uma constante chamada alunos que receberá a listaDeAlunosEMédia na posição 0:
Então, na atribuição de indice, substituiremos listaDeAlunosEMedia[0] por alunos. Assim, fica mais claro a que estamos nos referindo e a linha fica mais legível:
Vamos realizar um processo semelhante para listaDeAlunosEMedias[1]. Também no início do bloco if, criaremos uma constante chamada medias que recebe listaDeAlunosEMedias[1]:
Em seguida, na atribuição de mediaDoAluno, trocaremos listaDeAlunosEMedias[1] por medias:
Mas temos como melhorar ainda mias o nosso código! Ao declarar alunos e medias, fizemos atribuições partindo da mesma lista. Desde o JavaScript 6, existe uma maneira mais concisa de fazer essa atribuição. De início, vamos comentar as constantes alunos e medias:
Abaixo do trecho comentado, declararemos uma constante com uma sintaxe diferente. Vamos escrever const e, em lugar do nome, colocaremos um par de colchetes. Dentro deles, colocaremos alunos e medias, separados por vírgula. Atribuiremos listaDeAlunosEMedias a essa constante:


```bash
const [alunos, medias] = listaDeAlunosEMedias;
```


Essa nova linha equivale às duas linhas que comentamos há pouco. Quando abrimos e fechamos colchetes logo após uma declaração, como const, nós estamos nomeando cada um dos elementos da lista no lado direito da atrubuição. Em outras palavras, criamos uma constante chamada alunos para a posição 0 de listaDeAlunosEMedias e também criamos uma constante chamada medias para a posição 1 de listaDeAlunosEMedias. Funciona exatamente como as duas linhas comentadas.

Essa sintaxe diferenciada e específica do JavaScript chama-se sintaxe de desestruturação de listas. Ela nos ajuda a tornar o código mais conciso e é bastante utilizada no mercado! A desestruturação serve para outros tipos de dados do JavaScript.


```bash
const alunos = ["João", "Juliana", "Ana", "Caio"];
const medias = [10, 8, 7.5, 9];

const listaDeAlunosEMedias = [alunos, medias];

function exibeNomeENota(aluno){
    if (listaDeAlunosEMedias[0].includes(aluno)) {
        const [alunos, medias] = listaDeAlunosEMedias;

        const indice = alunos.indexOf(aluno);

        const mediaDoAluno = medias[indice];

        console.log(`${aluno} tem a média ${mediaDoAluno}.`);

    } else {
        console.log("Aluno não encontrado!");
    }
}

exibeNomeENota("Ana");
```


### **For Clássico**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/60e20abe-ffcf-40f2-8f6a-2bd9b6f83270)


*Desafio 9: For*

Imprima o índice e a lista com os seguintes números:

100, 200, 300, 400, 500, 600


*Sintaxe e funcionamento do for*


O for é constituído por três expressões dentro dos parênteses, separadas por ponto e vírgula. A primeira expressão é executada uma única vez. No nosso caso, temos let indice = 0 — a declaração de uma variável, inicializada com o valor 0. Quando o JavaScript interpreta todo o código que escrevemos nesse arquivo, ao chegar na estrutura for, ele executará essa expressão uma vez.

A segunda expressão é a condição de execução do bloco for ** e a terceira expressão será executada sempre ao final do bloco**. Vamos inserir alguns comentários no código (antes do for) para não nos esquecermos da proposta de cada um das três expressões:

Assim, primeiramente o JavaScript executa a expressão let indice = 0. Em seguida, ele adentra no bloco contido entre as chaves. No caso, o console.log(). Terminado o bloco, o JavaScript executa a terceira expressão dentro dos parênteses, incrementando o valor da variável indice. Se antes era 0, agora temos 1.

Com o novo valor de indice, a segunda expressão será interpretada — a condição de execução. Caso a condição seja satisfeita, o bloco entre chaves será executado novamente. Esse ciclo será repetido, até que a condição deixe de ser satisfeita. Executamos o console.log(). Terminado o bloco, executamos indice++. Agora, indice é igual a 2. Verificamos a condição de execução: 2 é menor que 6? Sim, então continuamos a repetição. Em dado momento, indice terá valor 6 e a condição de execução não será mais satisfeita.

Ao construir uma estrutura for, é importantíssimo atentar à condição de execução. Se ela nunca for invalidada, entramos em um loop infinito! Você pode ler mais a respeito na próxima atividade deste curso.

Portanto, essa é a composição e o funcionamento de um for clássico, essa estrutura presente em quase todas as linguagens de programação.

Cada execução do loop chama-se iteração. Então, na primeira iteração, imprimimos o indice quando ele tinha o valor 0. Na segunda iteração, imprimimos o indice quando ele tinha o valor 1, e assim em diante até o valor 5. Houve 6 iterações.

Como um toque final pra melhorar nosso código, na condição de execução do bloco for, podemos substituir o número 6 por um valor dinâmico. Em vez de 6, usaremos o tamanho do array:


```bash
const numeros = [100, 200, 300, 400, 500, 600];

// Primeira expressão: é executada apenas uma única vez
// Segunda expressão: condição de execução
// Terceira expressão: é executada sempre ao final do bloco

for (let indice = 0; indice < numeros.length; indice++) {
    console.log(numeros[indice]);
}
```

### **Loop infinito**


Os laços de repetição, como o for, são ferramentas essenciais na programação. São utilizados para, entre outras coisas, percorrer arrays e executar blocos de código para cada elemento.

Porém, quando usamos for para executar códigos em loop, temos que deixar claro qual é a condição de execução do loop. Caso contrário, o programa não sabe em que momento deve parar de executar o loop, acaba ficando “preso” e entrando em loop infinito.

O loop infinito pode travar seu navegador, o terminal em que o código estiver sendo executado, ou até mesmo o computador, então é importante saber como evitá-lo.

Abaixo temos um exemplo de for que imprime no terminal números de 0 a 10:


```bash
for (let indice = 0; indice <= 10; indice++) {
  console.log(indice);
}
```


O código executa corretamente e o programa é capaz de encerrar o loop, pois a condição de execução indice <= 10 está correta, a variável indice que faz o controle do loop começa em 0 e ao fim de cada ciclo do loop, é aumentada em 1 (indice++). Quando o valor da variável de controle indice chega a 11, depois de imprimir o número 10 no terminal, a comparação indice <= 10 se torna false e isso encerra o loop.

O loop infinito pode acontecer caso alguma das expressões seja passada de forma incorreta ou esteja faltando. Por exemplo a terceira, responsável por alterar indice após o bloco de código dentro do for ter sido executado:


```bash
for (let indice = 0; indice <= 10; ) {
  console.log(indice);
}
```


A mesma coisa acontecerá se o for for executado sem a segunda expressão, que é a condição de execução.


```bash
for (let indice = 0; ; indice++) {
  console.log(indice);
}
```


Outro caso que pode gerar loop infinito é o de alterações feitas na variável de controle dentro do bloco do for, o que não é uma boa prática:


```bash
for (let indice = 0; indice < 10; indice++) {
  indice--;
  console.log(indice);
}
```


IMPORTANTE: Como mencionamos acima, o loop infinito pode travar o terminal ou computador. Se durante seus estudos você perceber que executou um código com loop infinito, finalize a execução do programa o mais rápido possível no terminal pressionando “Ctrl + C”.



#### **Média com FOR**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/14013d6a-8465-4c4d-9a42-f0272899a9ae)


*Desafio 10: Média*


Calcule a média entre as seguintes notas, usando o for:

10
6.5
8
7.5


```bash
const notas = [10, 6.5, 8, 7.5];

let somaDasNotas = 0;

for (let i = 0; i < notas.length; i++) {
  somaDasNotas += notas[i];
}

const media = somaDasNotas / notas.length;

console.log(`A média das notas é ${media}.`);
```


#### *Loops em matrizes*


Vimos como usar os loops para percorrer um array utilizando ofor:


```bash
const notas = [10, 6.5, 8, 7.5];

let somaDasNotas = 0;

for (let i = 0; i < notas.length; i++) {
  somaDasNotas += notas[i];
}

const media = somaDasNotas / notas.length;

console.log(`A média das notas é ${media}.`);
```


Agora, se quisermos percorrer matrizes, um único for não será suficiente. Mas podemos usar o for várias vezes, uma para cada dimensão da matriz. Assim, uma matriz de duas dimensões usará dois for, um dentro do outro. Começaremos criando mais alguns arrays e uma matriz de 2 dimensões.


```bash
const notas1 = [10 , 6.5, 8 ,7.5]
const notas2 = [9  , 6  , 6]
const notas3 = [8.5, 9.5]
 
const notasGerais = [notas1,notas2,notas3]
 
let media = 0

```


Com a matriz criada, vamos iterar sobre os elementos. Mas não poderemos usar o mesmo for utilizado da última vez, já que agora notasGerais[i] contém um array e não mais um valor numérico. Por isso usaremos outro for para acessar esse array.


```bash
for (let i = 0; i < notasGerais.length; i++) {
  for (let j = 0; j < notasGerais[i].length; j++) {
    media += notasGerais[i][j]/notasGerais[i].length;
  }
}
```


Vamos entender um pouco melhor as partes que compõem esse código.

No primeiro for criamos uma let i e vamos executar o bloco de código enquanto i for menor que notasGerais.length. Como temos 3 elementos (nesse caso, arrays), o primeiro for será executado 3 vezes, com i=0,i=1,i=2.

O segundo for tem uma nova variável, a let j, já que não podemos usar uma nova let i porque ela já está definida, e vamos executá-lo enquanto j for menor que notasGerais[i].length. Como cada notasGerais[i] é um array, podemos obter a propriedade de tamanho dele utilizando o .length.

O código dentro do segundo for vai acumular o valor de notasGerais[i][j], lembrando que notasGerais[i] é um dos 3 arrays iniciais. Assim, o parâmetro [j] vai acessar o elemento dentro array escolhido pelo notasGerais[i], retornando um número que podemos usar na nossa conta.

Então ficamos com o seguinte código:


```bash
const notas1 = [10 , 6.5, 8 ,7.5]
const notas2 = [9  , 6  , 6]
const notas3 = [8.5, 9.5]
 
const notasGerais = [notas1,notas2,notas3]
 
let media = 0
 
for (let i = 0; i < notasGerais.length; i++) {
  for (let j = 0; j < notasGerais[i].length; j++) {
    media += notasGerais[i][j]/notasGerais[i].length;
  }
}
 
console.log(media)
```


No entanto, este código retorna uma média de 24. Como tal média é possível se não temos nenhum número maior do que 10? O que acontece é que para conseguir a média entre todos os arrays, temos que somar as médias dos arrays de notas, 8+7+9 e dividir pela quantidade de arrays em notasGerais.


```bash
const notas1 = [10, 6.5, 8 ,7.5]
const notas2 = [9, 6, 6]
const notas3 = [8.5, 9.5]
 
const notasGerais = [notas1,notas2,notas3]
 
let media = 0
 
for (let i = 0; i < notasGerais.length; i++) {
  for (let j = 0; j < notasGerais[i].length; j++) {
    media += notasGerais[i][j]/notasGerais[i].length;
  }
}
 
media = media/notasGerais.length
 
console.log(media)
```


Com isso usamos o for para passar por todos os elementos da matriz, e nesse caso, calcular a média dos valores deles.



#### **Media com FOR OF**


*Desafio 11: Média com for of*


Calcule a média entre as seguintes notas usando o for of:

10
6.5
8
7.5

Diferentemente do for clássico, o for of é composto por uma única expressão. Além disso, essa estrutura é caracterizada pelo of, que incluímos após let elemento. O termo of significa "de", em inglês.

Portanto, com essa expressão, é como se estivéssemos dizendo: para cada elemento de notas, execute o código que está dentro das chaves. O for of é muito adequado para utilizarmos com arrays.

No for clássico, nós mesmos declaramos uma variável de controle, a incrementamos manualmente e indicamos a condição para a continuidade (ou não) do loop, que será avaliada a cada iteração. Já no for of, o JavaScript automatiza alguns desses processos.

Quando queremos percorrer um array, podemos usar o for of. Assim, o JavaScript já entende que temos que percorrer o array do início ao fim. A grande vantagem dessa estrutura é que podemos selecionar diretamente o valor de cada elemento da lista e, por exemplo, imprimi-lo com um console.log(), como fizemos.

Usamos a palavra "elemento", porque é um termo genérico. Vamos renomeá-lo para um nome mais específico para nosso caso. Posicionaremos o cursor sobre elemento, pressionaremos a tecla "F2" e o renomearemos de "elemento" para "nota". Assim, o código ficará mais semântico:

O for of é uma forma mais concisa de escrever o for tradicional, mas depende da situação. Ele funciona em casos que precisamos percorrer uma lista do início ao fim, passando por todos os elementos.

O for clássico pode ter uma sintaxe mais complicada, porém ele também é mais flexível para abordar contextos mais complexos. Por exemplo, conseguimos percorrer um array de trás para frente, fazer um decremento na variável de controle e ou até aumentar essa variável de dois em dois, de três em três, caso não seja necessário passar por todos os itens da lista.

O for of não tem toda essa flexibilidade, contudo ele fornece uma sintaxe mais sucinta que serve para a maioria dos casos, quando o objetivo é percorrer um array completo.


```bash
const notas = [10, 6.5, 8, 7.5];

let somaDasNotas = 0;

for (let nota of notas) {
  somaDasNotas += nota;
}

const media = somaDasNotas / notas.length;

console.log(`A média das notas é ${media}.`);
```

#### **Possibilidades do for**


A estrutura for tem uma sintaxe mais complexa que o for of, com mais expressões, mas por causa disso fornece um maior leque de possibilidades de acordo com a nossa necessidade.

Por exemplo, podemos percorrer um array do fim ao início:


```bash
const numeros = [100, 200, 300, 400, 500, 600];

for (let i = numeros.length - 1; i >= 0; i--) {
  console.log(numeros[i]);
}
```


Declaramos o valor inicial da variável de controle como o valor da última posição do array `(numeros.length - 1)`; realizamos um decremento `(i--)` ao invés de um incremento e a condição de execução é `i >= 0`. Ou seja, nesse caso, a variável `i` começará do valor 5 e irá até 0.

Ao executar o código, no terminal aparecerá:


``` bash
600
500
400
300
200
100
```


Outra possibilidade é alterar a quantidade incrementada ou decrementada, utilizando o mesmo código acima, mas alterando o decremento para i -= 2. Então, teremos o seguinte:


```bash
const numeros = [100, 200, 300, 400, 500, 600];

for (let i = numeros.length - 1; i >= 0; i -= 2) {
  console.log(numeros[i]);
}
```


O valor de i será diminuído de 2 em 2 a cada iteração (lembrando que a expressão `i -= 2` equivale a `i = i - 2`). Assim, os valores de i serão 5, 3 e 1, e no terminal aparecerá:


```bash
600
400
200
```


Também temos controle sobre a condição de execução, então se alterarmos esse último código para ter a condição `numeros[i] > 300`, teremos o seguinte:


```bash
const numeros = [100, 200, 300, 400, 500, 600];

for (let i = numeros.length - 1; numeros[i] >= 300; i -= 2) {
  console.log(numeros[i]);
}
```


E no terminal aparecerá:


```bash
600
400
```


Por fim, até agora utilizamos a estrutura for apenas para percorrer arrays, mas ela pode ser utilizada para repetir qualquer instrução conforme a necessidade. Por exemplo, podemos criar dinamicamente um array com todos os números pares de 0 a 100:


```bash
const numerosPares = [];

for (let i = 0; i <= 100; i += 2) {
  numerosPares.push(i);
}

console.log(numerosPares);
```


No terminal aparecerá:


```bash
[
   0,  2,  4,  6,  8, 10,  12, 14, 16, 18, 20,
  22, 24, 26, 28, 30, 32,  34, 36, 38, 40, 42,
  44, 46, 48, 50, 52, 54,  56, 58, 60, 62, 64,
  66, 68, 70, 72, 74, 76,  78, 80, 82, 84, 86,
  88, 90, 92, 94, 96, 98, 100
]
```


Na maioria dos casos, você não precisará realizar repetições mais complexas como essas, mas nunca se sabe, certo? Por isso, conhecer os recursos de uma linguagem e suas possibilidades pode ser uma “mão na roda” no futuro.

Como vimos, para percorrer todos os elementos de um array e do início ao fim, o for of fornece uma sintaxe mais sucinta que o for.


## 6 FUNÇÕES CALLBACK


### **Média com FOR EACH**


*Desafio 12: Média com forEach*

Calcule a média entre as seguintes notas usando o forEach:

10
6.5
8
7.5

o forEach também é uma estrutura de repetição. 
Quando uma função é parâmetro de outra, chamamos a função passada como callback. Ou seja, essa função anônima também é callback nesse caso.
Em português, callback significa "chamar de volta". tem esse nome porque é uma função que estamos guardando de alguma forma na lógica interna do forEach e ela vai ser chamada de volta em determinados momentos.
Podemos perceber que o forEach tem uma lógica parecida com o for of, ele fornece diretamente o valor do elemento do array, que nesse caso nomeamos de nota, e ele também sempre vai do início ao fim do array.

Mas o forEach tem uma vantagem em relação ao for of. Nos parâmetros da função callback, podemos passar mais um parâmetro, usando uma vírgula entre os parâmetros.

Provavelmente, no mercado, você verá o forEach sendo bastante utilizado, até mais do que o for of.

```bash
const notas = [10, 6.5, 8, 7.5];

let somaDasNotas = 0;

notas.forEach(function (nota) {
  somaDasNotas += nota;
});

const media = somaDasNotas / notas.length;

console.log(`A média das notas é ${media}.`);
```


#### **for...of vs callbacks**


Até agora vimos várias formas de fazer o que parece ser a mesma coisa: for, for…of, forEach()... Com tantas opções, como posso escolher qual usar no meu código?

Antes, vamos dar uma olhada em cada um deles:

`for` - A forma mais “clássica” de se efetuar um loop em JavaScript e em várias outras linguagens, o for é muito conveniente pois pode ser utilizado com qualquer tipo de iterável e é construído de uma forma que deixa muito claro quais são todas as “fases” de cada loop - também chamamos um loop de laço de repetição ou de iteração.

`O que é um “iterável”?` Além de arrays, strings, sets (conjuntos) e maps (mapas ou dicionários) são considerados iteráveis. Não vamos falar dos dois últimos tipos neste curso, mas se você tiver interesse em saber mais sobre conjuntos, dicionários e outras estruturas de dados, pode dar uma olhada neste artigo; o que precisamos saber agora é que um iterável, aqui, representa uma sequência de elementos que pode ser percorrida (ou seja, iterada) utilizando ferramentas próprias para isso. É importante fazer uma distinção entre array e iterável, pois nem todo método que funciona em um array vai funcionar em outros iteráveis - veremos isso em seguida.


```bash
const lista = [1, 2, 3, 4, 5];

for (let indice = 0; indice < lista.length; indice++) {
 console.log(lista[indice]); 
}
```


O que queremos dizer com “deixar claro as fases da iteração” pode ser visto no exemplo acima: a expressão entre parênteses () após a palavra-chave for. Dentro da expressão temos:

uma variável contadora, que é criada antes do início do laço (let indice);
uma expressão de teste (indice < lista.length), que é executada antes de cada iteração e que verifica se o código dentro do bloco {} deve ou não ser executado;
por último, uma expressão que é executada ao final de cada laço, normalmente um incremento (++) ou decremento (--) da variável contadora.
Ou seja: como as fases de cada laço são declaradas de forma explícita, elas também podem ser alteradas conforme a necessidade do código, o que faz com que o for seja muito versátil e possa ser utilizado em casos específicos, quando os outras formas de sintaxe mais reduzida (como os que vamos ver em seguida) não atendem. O laço pode ser decremental ao invés de incremental (percorrer um array de trás para frente), a variável contadora pode receber outro valor como let indice = 2 ou let indice = outraVariavel + 1 (desde que esse valor seja avaliado como número), a condição de teste pode ser o tamanho do array como no exemplo, ou outro (indice < lista.length - 1) e o incremento ou decremento ao final do laço pode receber qualquer operador aritmético ou ser o resultado de uma operação, como indice = indice + 2 ou indice *= 2.


É possível, inclusive, usar o for para executar algoritmos mais complexos, que também não seriam possíveis com outros métodos, por exemplo:


```bash
const lista = [1, 2, 3, 4, 5];

for (let i = 0, j = 0; i < lista.length; i++, j++) {
 console.log(lista[i] + j); 
}

//1
//3
//5
//7
//9
```


Ainda há outras formas de se trabalhar com as condições do for, que você pode conferir na - [documentação sobre for](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/for) no MDN. 

`for…of` Adicionado às funcionalidades do JavaScript na versão ES6, é um tipo de laço de repetição diferente do for tradicional, embora utilize a mesma palavra-chave:


```bash
const lista = [1, 2, 3, 4, 5];
let soma = 0;

for (let elemento of lista) {
 soma += elemento;
}

console.log(soma)
```


O for…of pode ser executado utilizando qualquer tipo de iterável: além de arrays, strings, sets (conjuntos) e maps (mapas ou dicionários) são considerados objetos iteráveis. Não vamos falar dos dois últimos tipos neste curso, mas se você tiver interesse em saber mais sobre conjuntos, dicionários e outras estruturas de dados, pode dar uma olhada neste artigo; o que precisamos saber agora é que um iterável, aqui, representa uma sequência de elementos que pode ser percorrida (ou seja, iterada) utilizando o for…of. É importante fazer esta distinção entre array e iterável, pois nem todo método ou declaração que funciona em um array vai funcionar em outros iteráveis.


Olhando assim, o for…of se parece bastante com o for: temos a declaração de uma variável (let elemento) seguida da palavra-chave of e um identificador do iterável que será percorrido (no caso acima é um array mesmo, lista).


A diferença principal e mais visível entre o for e o for…of é que o anterior dá muito mais controle sobre de que forma o laço de repetição ocorre. Por exemplo, vimos que no for é possível manipular de forma mais fina todas as condicionais; já no for…of as condições são mais “fixas”: elemento se refere a cada elemento (ou item) do array e o loop sempre ocorre de forma sequencial, do primeiro elemento até o último.


Em contrapartida, a sintaxe simplificada e mais “legível” para pessoas faz com que o uso do for…of seja mais prático do que o for, pois laços de repetição mais simplificados, que percorrem um iterável do primeiro ao último elemento e executam o código do bloco a cada iteração, são muito mais corriqueiros.


#### *** `forEach()` ***


Ao contrário de for e for…of, o forEach() é um método do objeto Array.


O que é um -[método](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Functions/Method_definitions)? Em programação, chamamos de método uma função que é propriedade de um objeto. A documentação do MDN traz alguns exemplos de métodos, mas você vai poder conferir com mais detalhes o que são objetos e suas propriedades quando fizer o curso de fundamentos do JavaScript: Objetos. Por agora, basta saber que quando dizemos que determinada função - por exemplo, forEach() é um método de array, significa que esta função foi desenvolvida para trabalhar apenas com esse tipo de dado - no caso, com arrays.


O forEach(), assim como outros métodos de array que vimos ou ainda vamos ver durante esta aula, também cumprem o papel de iterar arrays, porém com funcionalidades e retornos bem definidos. No caso do forEach(), apesar da sintaxe bem diferente, podemos utilizar este método como o for ou o for…of, pois ele vai executar as instruções que forem passadas para cada elemento iterado, sem retornar nenhum dado.


O - [forEach()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array), assim como alguns outros métodos de array do JavaScript que estamos vendo no curso, utiliza a abordagem funcional de funções callback para executar o código necessário a cada elemento iterado no laço:


```bash
const lista = [1, 2, 3, 4, 5];
let soma = 0;

lista.forEach(numero => soma += numero);
console.log(soma)
```


Como visto acima, o método forEach() recebe uma função como parâmetro, e esta função por sua vez utiliza como parâmetro cada um dos elementos do array. A lógica interna do forEach() vai manejar a iteração do primeiro ao último item do array e fazer com que o código definido dentro da função callback (no caso, apenas um incremento soma += numero) seja executado a cada iteração.


O mesmo código também poderia ser escrito da seguinte forma, um pouco mais extensa porém mais legível:


```bash
lista.forEach(numero => {
 soma += numero
});
```


Ou ainda, utilizando a palavra-chave function ao invés de arrow functions; essa forma de escrita não é usual, pois quando usamos funções callback o padrão adotado é o de arrow functions, mas serve para o propósito de legibilidade:


```bash
lista.forEach(function (numero) {
 soma += numero
});
```


Assim, vemos que o forEach() não retorna nenhum tipo de valor, apenas executa o que está dentro do bloco da função callback, assim como for e for…of. Porém também não é possível modificar a forma que a iteração será feita (é sempre do primeiro elemento do array ao último) e não há forma de interromper o laço dada alguma condição, como o break funcionaria para um for normal.

O forEach() também não pode ser utilizado com qualquer iterável, apenas com arrays e também não pode ser utilizado de forma assíncrona - um tema um pouco mais avançado e que não trabalharemos nesse curso, mas que você pode conferir - [neste artigo](https://www.alura.com.br/artigos/async-await-no-javascript-o-que-e-e-quando-usar?_gl=1*1hxko04*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwNTMzODQ1OC4xNi4xLjE3MDUzNDA0OTYuMC4wLjA.*_fplc*dW9uU0VaVkprRURiWDduU043TzUwWE4zNllKUFczMG4lMkJyM2FsMVdJUW1sNzhVbENibDZ0VFRYUGtFdG1ZR29COHdXNG5CYURnQTJKMUtnZVRuaU56TElPbldVakxyMHp5MzE3MW9uY2YxNGZEUEx2cHMlMkJGaWtqZWlJZXRKZyUzRCUzRA..) se tiver curiosidade pra começar a aprender.

Atualmente, em termos de performance - ou seja, qual código é executado de forma mais rápida pelo computador e consumindo menos recursos de memória - tanto os laços com for como o forEach() não tem diferenças significativas, embora ainda possam ocorrer exceções, como no caso de versões muito antigas de navegadores e/ou manipulação de arrays muito longos. Mas no momento em que desenvolvemos este curso a questão de performance não é tão definidora na maior parte dos casos, pois os interpretadores do JavaScript já evoluíram para trabalhar tão bem com funções callbacks quanto com iteradores.

O forEach() utiliza callbacks assim como map(), filter() e alguns outros métodos de array, o que facilita a utilização desses métodos em conjunto ou a troca de um para outro dependendo da necessidade do código ou de uma refatoração. Alguns guias de estilo de código desenvolvidos pela comunidade, como o famoso - [guia do AirBNB](https://github.com/airbnb/javascript#iterators-and-generators), indica preferencialmente o uso do forEach() no lugar do for…of para manter a consistência no estilo do código.

O for…of, mais recente que o forEach(), não é um método de array e sim um iterador, assim como o for. Ou seja, vai trabalhar com outros tipos de dados iteráveis além de arrays, com uma sintaxe mais simplificada que a do for.

Como em ambos os casos não há retorno, somente a execução do código que está dentro do bloco - os colchetes {} do for…of ou a função callback do forEach(), você pode utilizar as ferramentas da seguinte forma:

forEach() para trabalhar com arrays da forma mais corriqueira - percorrendo do primeiro ao último elemento, sem alterar a condição de parada, e também para manter a coesão do estilo quando em conjunto com outros métodos de array como map, filter e etc;
for…of em caso de iteráveis (dicionários, conjuntos e outras estruturas de dados) ou de arrays quando for necessário o uso de programação assíncrona e/ou dar condições de saída do laço (por exemplo, com o uso de break);
for para casos em que seja necessário manipular de forma mais fina as fases do laço (condição inicial, condição de parada e incremento).



#### **Método map()**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/a44bd41c-e51c-471d-9488-869cae9f9115)


*Desafio 13: ponto extra*

Um aluno recebeu um ponto extra nas suas notas. Adicione esse ponto nas notas da seguinte lista:

`
10
9.5
8
7
6
`

O map() também é uma estrutura de repetição do JS, ele vai executar essa função callback para cada uma das notas e para cada uma vai atribuir um novo valor.

O map() é muito apropriado para reescrever arrays, que é justamente o que queremos neste desafio.

o map() não altera o array original.

O map() não substitui o forEach(), ele não consegue abranger todas as situações do forEach(). Porém, ele é muito útil nos casos em que queremos reescrever um array e alterar todos os valores de alguma forma.


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/f60945d3-cdc8-4fed-8550-569a6f32551b)



Poderíamos usar um loop para percorrer todas as letras de um string?

“String”, além de ser o tipo de dado usado para representar textos, também se define como uma sequência ordenada de caracteres!

“Lista ordenada” (ou sequência) também é uma forma de definir arrays, certo? Então podemos pensar que, por baixo dos panos, strings são armazenadas em memória da seguinte forma:


```bash
const nome = "Alura";
// ["A", "l", "u", "r", "a"]
```


Ou seja, é possível utilizar alguns métodos de array e laços de repetição para acessar e alterar strings:


```bash
const nome = "Alura";
let nomeMaiusculas = "";

for (let i = 0; i < nome.length; i++) {
 nomeMaiusculas += nome[i].toUpperCase()
}
console.log(nomeMaiusculas) //ALURACOPIAR CÓDIGO
const nomedoCurso = "Fundamentos de JS";
const nomeDaPlataforma = " Alura"

const nomeCompleto = nomedoCurso.concat(nomeDaPlataforma)
console.log(nomeCompleto)  //Fundamentos de JS Alura
```


Você pode conferir a lista completa de métodos de string na - [documentação do MDN]( https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String#methods) .


#### **map() e forEach**


Agora já vimos mais sobre as funções callback e o método map() que utiliza essas funções, também vimos anteriormente sobre o método forEach().

Qual a principal diferença entre os métodos map() e forEach()?

métodos callback**


Nesta aula introduzimos um novo conceito, o de funções callback.

O termo callback se refere à função que é “chamada de volta” dentro de outra função. Após o lançamento do ES6 (também conhecido como EcmaScript 2015) o uso desse tipo de método foi se consolidando, então é importante entender como utilizá-lo.

O JavaScript moderno traz vários métodos e funções callback diversos, não apenas para uso com arrays. Porém a estrutura da função se mantém similar.

Crie um novo arquivo index.js e crie uma array de números:


```bash
const arrayNums = [1, 2, 3, 4]
```

Vamos utilizar o map() para multiplicar cada um dos valores nesse array por 10 e retornar um novo array com os resultados. Antes de escrevermos o map() para isso, vamos criar a função callback; ou seja, a função que vamos chamar (call) de volta quando executarmos o método map():


```bash
function multiplicaPorDez(num) {
 return num * 10
}
```


Agora podemos chamar o map() para fazer a operação:


```bash
const arraySomada = arrayNums.map(multiplicaPorDez)

console.log(arraySomada)
```


O resultado no terminal deve ser `[ 10, 20, 30, 40 ]`.

IMPORTANTE: Observe a função multiplicaPorDez. Quando criamos esta função, especificamos que ela precisa receber o parâmetro (num) para ser executada corretamente. No entanto, quando ela está sendo chamada dentro de arrayNums.map(), não passamos nenhum parâmetro e mesmo assim funcionou. O que aconteceu aqui?

Para entender melhor, vamos reescrever o código, passando a função multiplicaPorDez(num) direto como parâmetro do map():


```bash
const arraySomada = arrayNums.map(num => num * 10)

console.log(arraySomada)
```


No código acima, substituímos uma função externa e nomeada (a função multiplicaPorDez), por uma arrow function anônima que existe somente dentro do map(). Mas esta função anônima também tem um parâmetro, num, que representa cada um dos elementos do array que será iterado pelo map().

Por isso, quando utilizamos uma função externa como callback de um map(), não foi necessário passar um parâmetro. O map() executa automaticamente o bloco de código da função (nesse caso, num * 10) para cada elemento do array.

Ambos os casos de uso são válidos; as funções externas permitem reaproveitamento de código, mas há vários momentos em que isso não será necessário.

Para o JavaScript, qualquer função que seja chamada como argumento de outra é considerada uma função callback, não apenas em caso de métodos. Você pode ver outros exemplos no [MDN](https://developer.mozilla.org/pt-BR/docs/Glossary/Callback_function).


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/7efcda38-08b1-4740-a015-bb81e24ee1f6)


## 7 AVANÇANDO EM ARRAYS

### 7.1 **Filtrando Elementos**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/32d89e5f-d4b7-4d52-a549-6e97c2335967)


*Desafio 15: filtrando por nota*

Depois de calcular a média dos alunos, precisamos mostrar quem está reprovado entre os alunos:


```
Ana: 7
Marcos: 4.5
Maria: 8
Mauro: 7,5
```


Poderíamos, por exemplo, usar o forEach(), dentro do forEach() usar o slice() para modificar o array e mostrar as pessoas reprovadas.

Porém, nesta situação específica podemos usar um método moderno que se chama filter(), que em português significa "filtrar". Queremos realmente filtrar essa lista pelos alunos reprovados.

O filter() retorna um novo array. Então vamos escrever que const reprovados recebe alunos.filter(). Queremos filtrar a lista de alunos, por isso aplicamos o filter() em alunos.

não estamos usando o parâmetro aluno, porque dessa vez estávamos interessados apenas no índice. Quando não utilizamos o primeiro parâmetro, uma convenção que você pode encontrar é o uso do underline (_) em vez de nomear o parâmetro, então em vez de alunos.filter(aluno, indice) fica alunos.filter(_, indice). Só de fazer isso o JS vai saber que não estamos utilizando esse parâmetro.

É apenas uma convenção da linguagem, não é obrigatório fazer isso. Mas é obrigatório nomear o primeiro parâmetro de alguma forma para podermos acessar o segundo parâmetro, o índice.


```
const alunos = ["Ana", "Marcos", "Maria", "Mauro"];
const medias = [7, 4.5, 8, 7.5];

const reprovados = alunos.filter((_, indice) => {
  return medias[indice] < 7;
});

console.log(reprovados);

```


### **Retorno do filter**


Vimos como utilizar o método filter para retornar um array com apenas alguns elementos do array principal através de uma função callback.

O que deve ser retornado da função callback para que o método filter funcione?


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/6e1713d1-1e81-465b-80b6-d17ea1eb3f94)



### 7.2 **Somando com Reduce**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/7bce3347-3494-43a6-9f6d-b5e2719759ad)


*Desafio 16: médias das turmas*

Com a média de todos os alunos de 3 salas, calcule a média geral de cada sala:


```bash
const salaJS = [7, 8, 8, 7, 10, 6.5, 4, 10, 7];

const salaJava = [6, 5, 8, 9, 5, 6];

const salaPython = [7, 3.5, 8, 9.5];
```


Já vimos como calcular média antes com o forEach(), mas essa lógica de ter uma variável que começa em zero e vai incrementando aos poucos, tem um método que vai nos ajudar nesse caso de somar vários números de uma lista.

O reduce não altera o array original, então precisaremos retornar o valor de reduce para uma nova variável.

Num primeiro momento o reduce pode parecer um pouco mais complicado, ele tem uma lógica bem interna, abstrai bastante coisa. Mas, resumindo, usamos o acumulador, informamos o valor inicial dele no segundo parâmetro do reduce e vamos atualizando o valor do acumulador a cada iteração que fazemos na lista.

Por fim, o parâmetro acumulador também é muito chamado de acc, que é uma abreviação do nome dele em inglês. E também podemos usar diretamente o retorno da função arrow function, em vez de usar a palavra return, vamos fazer essas modificações no nosso código:


```bash
const salaJS = [7, 8, 8, 7, 10, 6.5, 4, 10, 7];
const salaJava = [6, 5, 8, 9, 5, 6];
const salaPython = [7, 3.5, 8, 9.5];

function calculaMedia(notasDaSala) {
  const somaDasNotas = notasDaSala.reduce((acc, nota) => acc + nota, 0);

  const media = somaDasNotas / notasDaSala.length;

  return media;
}

console.log(`A média da sala de JavaScript é ${calculaMedia(salaJS)}`);
console.log(`A média da sala de Java é ${calculaMedia(salaJava)}`);
console.log(`A média da sala de Python é ${calculaMedia(salaPython)}`);
```

#### **estrutura do reduce()**


Durante a aula trabalhamos com o método reduce() para “reduzir” uma lista de números para um único valor. Este método trabalha com parâmetros um pouco diferentes dos outros que vimos durante o curso. Por isso, vamos destrinchar o exemplo da aula para entender melhor as partes do código.

Em seu editor, crie um arquivo index.js e execute o seguinte código:


```bash
const numeros = [43, 50, 65, 12]

const soma = numeros.reduce((acc, atual) => atual + acc, 0)

console.log(soma)
```


O código acima é muito parecido com o que foi feito durante a aula. É importante notar que:

O método reduce() está trabalhando com dois parâmetros. O primeiro é a função callback obrigatória para retornar o cálculo e o segundo parâmetro é um número que representa o valor inicial do acumulador – no caso, 0.
A função callback foi escrita diretamente dentro do reduce(), e esta função também está recebendo dois parâmetros, ambos obrigatórios: o valor acumulado e o valor atual.
A função callback foi escrita na forma de arrow function; nesse caso, quando só temos uma linha de instrução dentro da função (atual + acc) não precisamos usar chaves e nem da palavra-chave return.
Caso você tenha mais de uma linha de instrução dentro de uma arrow function, as chaves {} e a palavra-chave return voltam a ser necessários.

Vamos reescrever o reduce() de uma forma um pouco mais extensa para separar melhor as partes do código:


```
const soma = numeros.reduce(function (acc, atual) {
 return atual + acc
}, 0)
```


Vendo o código acima, percebe-se melhor onde começam e terminam cada um dos parâmetros do reduce(): o primeiro parâmetro, uma função e o segundo, um número.

Uma terceira forma de reescrever seria escrevendo a função callback fora do reduce():


```
function operacaoNumerica(acc, atual) {
 return atual + acc
}

const soma = numeros.reduce(operacaoNumerica, 0)
```


O reduce() roda o loop no array “por baixo dos panos”, executando para cada elemento a instrução passada na função operacaoNumerica.

No dia a dia, a forma que utilizamos no vídeo é a mais usual. Porém, durante seus estudos, você pode praticar da forma que achar mais clara.

É importante lembrar que cada método pode aceitar receber parâmetros diferentes! Alguns são obrigatórios, outros opcionais. Consulte sempre a documentação da linguagem.



### 7.3 **Clonando com spread operator**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/2f43d3cd-c237-4142-b40d-878a324e3d68)


Se queremos criar um novo array, sem alterar o original – que realmente é uma situação que acontece muito no dia a dia, às vezes queremos pegar o array original e fazer uma modificação para outros propósitos e sem alterar o original.

A primeira coisa que pensamos em fazer é escrever, por exemplo, const novasNotas = notas e fazer um push para adicionar o 10 no final do array.


Ao fazer uma atribuição direta como essa, usando o sinal de igual, o JavaScript entende que a partir desse momento, é como se esses dois arrays fossem o mesmo, como se eles apontassem para o mesmo endereço da memória.

Então, qualquer alteração que fizermos em novasNotas será feita no array original e vice-versa. É como se, para o JavaScript, eles fossem o mesmo array. E não é isso que queremos.

Nós queremos fazer uma cópia do array, mas sem que eles estejam tão interligados assim. Para resolver isso, na linha da atribuição coloremos notas dentro de colchetes e acompanhado de três pontos (...), como reticências.


```bash
const novasNotas = [...notas];
```


Esse é um operador do JavaScript que se chama spread operator, ou "operador de espalhamento". Ao utilizá-lo junto com uma lista, ele pega todo o conteúdo desse array e espalhar seus valores no local que estamos indicando. É como se copiássemos o conteúdo da lista, "7, 7, 8, 9", e colássemos no lugar do [...notas]. É isso que estamos dizendo para o JavaScript.

Então, o spread operator é um operador que podemos usar para clonar arrays sem ter problemas de referências do JavaScript.


```bash
const notas = [7, 7, 8, 9];

const novasNotas = [...notas, 10];

console.log(`As novas notas são ${novasNotas}`);
console.log(`As notas originais são ${notas}`);
```


**valor ou referência?**


No vídeo anterior, você viu como clonar um array de forma apropriada no JavaScript. Atribuir diretamente um array para outro com o sinal = faz com o que o JavaScript entenda que é como se eles fossem o mesmo array. Para evitar esse comportamento, devemos criar um array totalmente novo, com a ajuda do spread operator ... (ou operador de espalhamento).

Porém, esse comportamento não acontece com strings, números e booleanos, que são tipos primitivos do JavaScript.

Considere o seguinte código:


```bash
let num1 = 10;
let num2 = num1;

num2 += 5;
num1 += 1;

console.log(`Num1 é ${num1}. Num2 é ${num2}`);
```


Ao executar o código, teremos a frase “Num1 é 11. Num2 é 15”. Ou seja, com o código let num2 = num1, o JavaScript entende que queremos criar uma cópia de num1, e cria uma nova variável, com seu próprio espaço na memória guardando seu valor. Então, ao modificar uma das variáveis, a outra não é alterada.

Esse comportamento de copiar um valor primitivo, o atribuindo a uma nova variável, é chamado de atribuição por valor e acontece somente com os tipos primitivos do JavaScript.

O mesmo comportamento ocorre quando trabalhamos com parâmetros de funções. Veja o seguinte exemplo:


```bash
let numeroOriginal = 10;

function alteraNumero(numero) {
  numero = 50;

  console.log(`numero do parâmetro é ${numero}. numeroOriginal é ${numeroOriginal}`);
}

alteraNumero(numeroOriginal);
```


Executando o código, teremos a frase “numero do parâmetro é 50. numeroOriginal é 10”. Ao chamar a função passando numeroOriginal como parâmetro, foi feita uma cópia de seu valor para ser utilizada como o parâmetro numero dentro da função. Dessa forma, mesmo alterando numero dentro da função, numeroOriginal permanece inalterado.

Mas como você viu, com arrays não funciona bem dessa forma, afinal, eles não são um tipo primitivo. Considere o exemplo utilizado no vídeo passado:


```bash
const notas = [7, 7, 8, 9];

const novasNotas = notas;

novasNotas.push(10);

console.log(`As novas notas são ${novasNotas}`);
console.log(`As notas originais são ${notas}`);
```


A partir do código const novasNotas = notas, o JavaScript entende que novasNotas e notas passam a ser o mesmo array, e agora eles apontam para o mesmo espaço na memória. Como estamos lidando com dados mais complexos, o JavaScript faz isso por padrão para otimizar memória e performance, em vez de realizar uma cópia do array em toda nova atribuição.

Uma atribuição de um array é chamada de atribuição por referência, pois nela é passada a referência do array em si, e não uma cópia de seu valor.

O mesmo comportamento ocorre quando trabalhamos com parâmetros de funções. Veja o código abaixo:


```bash
const arrayOriginal = [7, 7, 8, 9];

function alteraArray(array) {
  array.push(10);

  console.log(`array do parâmetro é ${array}`);
  console.log(`arrayOriginal é ${arrayOriginal}`);
}

alteraArray(arrayOriginal);
```


Executando o código, teremos essa saída:


```bash
array do parâmetro é 7,7,8,9,10
arrayOriginal é 7,7,8,9,10
```


Após passar arrayOriginal como parâmetro de alteraArray, o utilizamos como o parâmetro array. O código array.push(10) alterou ambos os arrays, assim como o que houve no exemplo que fizemos a atribuição. Ou seja, novamente, foi passada a referência do array em si, e não uma cópia dele.

De forma análoga à solução do vídeo, caso queiramos passar uma cópia do array e não sua referência, trocamos o código alteraArray(arrayOriginal) por alteraArray([...arrayOriginal]). Assim, a saída será:


```bash
array do parâmetro é 7,7,8,9,10
arrayOriginal é 7,7,8,9
```


### 7.4 **Removendo Elementos Repetidos**


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/4582aa7f-f016-4f3c-9c2c-e9732d06f477)


Um professor acidentalmente adicionou nomes repetidos na lista de chamada:

```
Ana
Clara
Maria
Maria
João
João
João
```

Remova os nomes repetidos, deixando apenas um de cada.

Vou mostrar uma forma mais facilitada que o JS oferece com uma estrutura chamada Set, que em português significa "conjunto".
Para criar um novo Set vamos escrever const meuSet = new Set().

A palavra "new" em português significa "novo", é como se tivéssemos escrito "quero criar um novo Set".

Esse Set é uma classe do JavaScript, usaremos uma classe porque ela já vem com algumas lógicas internas.

O Set bem parecido com as listas que trabalhamos até agora, mas tem algumas regras a mais. Uma delas é que os elementos de um Set não podem se repetir. O que é ótimo para nos ajudar nesse desafio.

Para criar um Set com valores iniciais podemos passar uma lista dentro do parênteses de Set(). Vamos testar colocando alguns números e alguns deles reeptidos: "1, 1, 2, 3, 4, 4". e um console.log(meuSet) para vermos o que vai acontecer no meuSet.

Para finalizar, existe uma forma mais concisa de escrevermos esse código. Em vez de fazer [...meuSet] poderíamos colocar diretamente um new Set(nomes): [...new Set(nomes)] e apagar a linha em que declaramos o meuSet.


```bash
const nomes = ["Ana", "Clara", "Maria", "Maria", "João", "João", "João"];

const nomesAtualizados = [...new Set(nomes)];

console.log(nomesAtualizados);
```


Usando o `[...new Set(nomes)]` fazemos duas coisas ao mesmo tempo: passamos os nomes como valor de entrada do Set e os espalhamos para um novo array.


#### **estrutura Set**


Você viu que a estrutura Set é muito semelhante aos arrays, mas possui diferentes métodos e a interessante regra de que seus elementos não podem se repetir. Utilizamos essa regra ao nosso favor para eliminar as duplicatas de um array, convertendo-o para um Set e de volta para um array.

Você pode explorar mais seus conhecimentos sobre o Set na - [documentação](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Set).


## 8 OBJETOS

### 8.1 O que são objetos?


#### Adicionando e Alterando


TypeError: Assignment to constant variable.

Em português, atribuição à variável constante. Logo, isso é o que não podemos fazer, mas se tivermos um objeto armazenado em uma variável constante, podemos manipulá-lo, porém, não podemos reatribuir algum valor naquela variável.

#### Tipos de variáveis e objetos


Podemos alterar e manipular as propriedades de um objeto mesmo quando o objeto está armazenado em uma variável do tipo const.

Temos um [artigo](https://www.alura.com.br/artigos/entenda-diferenca-entre-var-let-e-const-no-javascript?_gl=1*1i9md25*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwNjIwMjc0NC4yNy4xLjE3MDYyMDQ3NjYuMC4wLjA.*_fplc*SVZPSGslMkJQNlMyc2UxT2NCTmllYyUyQjEyVkslMkJLVzdGZUJWSko1cHY4akxYdFhwSjB2c3AlMkZ1RGdxTWxjY0FaZmVWeXJuWXRhZmNvUE9kcHd5WDY2MHpVTTNOblQlMkJlSElTYkJPYlZkaGp1VE9nZSUyRjR1YjQxU1FBNVRXS3dkazdnJTNEJTNE) na plataforma que explica as diferenças entre as variáveis que podemos declarar, mas vale lembrar que as variáveis do tipo const apenas não podem ser reatribuidas, mas podem ter seu conteúdo interno alterado.


#### como deletar uma propriedade?


Já vimos como acessar, alterar e adicionar valores em um objeto. Mas ainda faltou falarmos sobre um caso: e quando queremos deletar um conjunto de chave/valor?

Vamos considerar o objeto abaixo:

```
const objPersonagem = {
 nome: "Gandalf",
 classe: "mago",
 nivel: "20",
 aliado: {
   nome: "Saruman",
   classe: "mago"
 },
 status: "desaparecido"
}
```

Se quisermos, por exemplo, remover a propriedade aliado, podemos utilizar o operador delete:
```
delete objPersonagem.aliado

console.log(objPersonagem.aliado) //undefined
```


Também é possível utilizar a notação de colchetes:

```
delete objPersonagem.aliado
delete objPersonagem["status"]

console.log(objPersonagem.aliado) //undefined
console.log(objPersonagem.status) //undefined
```

*Importante!* Veja que o delete remove do objeto o valor da propriedade, assim como a chave.

Após remover as duas propriedades acima, o objeto agora está desta forma:

```
{
 nome: "Gandalf",
 classe: "mago",
 nivel: "20",
}
```


O valor de retorno do operador delete é um booleano, ou seja, retorna sempre true ou false para cada operação. Porém, é importante notar que ele não retorna false se tentarmos remover, por exemplo, uma propriedade que não existe no objeto:


```
const delProp = delete objPersonagem.aliado
const delPropInexistente = delete objPersonagem["endereco"]

console.log(delProp) //true
console.log(delPropInexistente) //true

```


### 8.2 Manipulação de Objetos


#### Tipos de Dados e Valores


#### Objetos em Objetos


#### Listas de Objetos

#### Funções


#### objeto literal e referência


Vimos anteriormente como é a estrutura de um objeto, com seus pares de chave e valor:


```
const objPersonagem = {
 nome: "Gandalf",
 classe: "mago",
 nivel: "20"
}
```


O exemplo acima, assim como o que estamos criando durante esta aula, é o de um objeto literal.

Um objeto literal é um objeto criado com a notação literal, ou seja: uma lista de chave e valores dentro de chaves{ }, que atribuímos a uma variável para que o valor possa ser acessado depois. Exatamente como no exemplo acima.

Objetos literais funcionam bem quando queremos ter um objeto único com seus próprios dados. Isso porque um objeto literal sempre aponta para um mesmo local na memória, mesmo se você criar cópias dele. Vejamos o código a seguir:

```
const objPersonagem = {
 nome: "Gandalf",
 classe: "mago",
 nivel: "20"
}

const objPersonagem2 = objPersonagem
```


Se alterarmos apenas o objPersonagem2, o resultado é:


```
const objPersonagem2 = objPersonagem
objPersonagem2.nome = "Gandalf, o Cinzento"

console.log(objPersonagem.nome) //Gandalf, o Cinzento
console.log(objPersonagem2.nome) //Gandalf, o Cinzento

```


A variável objPersonagem2 não fez uma cópia do objeto original, apenas serviu como referência para o objeto original objPersonagem. Assim, qualquer alteração em qualquer um dos objetos altera ambos. Isso porque o JavaScript, quando trabalha com objetos, acessa os valores deles fazendo referência ao original. mas não cria uma cópia. Já o acesso por cópia funciona com tipos primitivos (string, number, booleano, null, symbol):


```
let num = 50
let num2 = num

num2 = 100
console.log(num) //50
console.log(num2) //100
```


Como podemos contornar esse comportamento quando criamos objetos? Além de utilizar a notação literal, objetos também podem ser criados através do método Object.create():


```
const objPersonagem = {
 nome: "Gandalf",
 classe: "mago",
 nivel: "20"
}

const objPersonagem2 = Object.create(objPersonagem)
objPersonagem2.nome = "Gandalf, o Cinzento"

console.log(objPersonagem.nome) //Gandalf
console.log(objPersonagem2.nome) //Gandalf, o Cinzento
```


O método Object.create() cria um novo objeto utilizando como protótipo o objeto passado via parâmetro. Dessa forma, objPersonagem2 é uma instância diferente de objPersonagem e pode ser trabalhada de forma independente.

Você pode ver mais exemplos desse método na [documentação do MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Object/create).



Um objeto pode conter um array de objetos, o que nos permite invocar desde funções comuns até arrays como filter().


### 8.3 Percorrendo Objetos

#### FOR...IN


o método for … In que permite a iteração sobre as propriedades de um objeto como em um array. 


![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/687561dd-c94e-46ad-8cf1-397b5ab32bac)


traz as chaves, nomes de nossas propriedades.

se utilizar:


```
console.log(cliente[chave])
```


acessa os valores de cada chave.



![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/58ec18e8-8c66-4e22-b10a-c65a2b4dbb6c)



se utilizar:


```
console.log(`A chave ${chave} tem o valor ${cliente[chave]}`)
```


ele trás cada chave e o valor de cada uma.



![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/9e4a8aa3-ae4e-4641-9d26-ea3c36b38149)



Para solucionar o erro que aparece na chave enderecos:



![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/6261da20-2b71-4141-b404-58ed6b99e7b8)



trazendo apenas o que é objeto.


#### METODOS DE OBJETO



![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/481bbbc5-4b70-4b0f-acd0-338d07d90940)



Aparecem as chaves:


![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/4c9d1c59-4dd0-40a6-ba76-b0f418e34ea9)



![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/bbb23827-83e7-4924-91eb-2004c518ff4a)


#### outros métodos de objetos



Acesse a [documentação do MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Working_with_Objects) e amplie os conhecimentos dos métodos e práticas que realizamos até agora.

Sabemos que o ecossistema JavaScript é bem vasto e sofre diversas mudanças em função do tempo, então vale a pena dedicarmos um tempo para olhar a documentação e dar uma lida com calma.



####  SINTAXE DE ESPALHAMENTO


serve para compor ou descompor arrays.


![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/25d8eae0-bb98-4de2-8245-5a983c385d8b)


ou, utilizando a sintaxe de espalhamento:


![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/d1bccf3c-8352-4b74-a18b-6843ad0f1a4d)


#### spread operator


Anteriormente, vimos um exemplo de uso do spread operator, também conhecido como sintaxe de espalhamento ou operador de espalhamento. Este operador copia as propriedades de objetos para outros, “espalhando” os conteúdos. Para entender melhor, vamos ver mais alguns exemplos:

```
const fichaGuerreiro = {
 nome: "Aragorn",
 classe: "guerreiro"
}

const equipoGuerreiro = {
 espada: "Andúril",
 capa: "capa élfica +2"
}
```


Ainda usando o exemplo acima, agora vamos tentar juntar esses dois objetos em apenas um, que vamos chamar de personagens. Em um primeiro teste, vamos criar um novo objeto literal com { } e passar para este objeto as variáveis de cada personagem:


```
const guerreiro = { fichaGuerreiro, equipoGuerreiro }
console.log(guerreiro)
```


O resultado no console não é exatamente o que queremos, pois os objetos ainda estão separados. Porém, agora o nome de cada variável é uma chave e o valor da chave é cada um dos objetos:


```
{
  fichaGuerreiro: { nome: 'Aragorn', classe: 'guerreiro' },
  equipoGuerreiro: { espada: 'Andúril', capa: 'capa élfica +2' }
}
```


Aqui é onde vamos utilizar o spread operator, adicionando a sintaxe de três pontos (reticências) antes do nome de cada objeto literal, separando-os com uma vírgula:


```
const guerreiro = { ...fichaGuerreiro, ...equipoGuerreiro }
console.log(guerreiro)COPIAR CÓDIGO
Após usar o spread operator, o console vai mostrar o resultado esperado, que é:

{
 nome: 'Aragorn',
 classe: 'guerreiro',
 espada: 'Andúril',
 capa: 'capa élfica +2'
}
```


*Importante!* Vale notar que, caso a sintaxe de espalhamento seja usada em objetos que tenham chaves/propriedades com o mesmo nome, o JavaScript vai sobrescrever o valor destas propriedades à medida que encontra novos valores com o mesmo nome de chave. Por exemplo:


```
const mago = {
 nome: "Gandalf",
 classe: "mago"
}
 const guerreiro = {
 nome: "Aragorn",
 classe: "guerreiro"
}

const ranger = {
 nome: "Legolas",
 classe: "ranger"
}
```


Os três objetos acima têm as mesmas propriedades. Mas o que acontece se tentarmos “espalhar” os dados em um único objeto com o spread operator? Vamos ver:

```
const personagens = { ...mago, ...guerreiro, ...ranger }
console.log(personagens)
```


Fazendo isso o resultado não será bem o que esperamos:

```
{ nome: 'Legolas', classe: 'ranger' }
```


Perceba que o JavaScript sobrescreve as chaves com o mesmo nome a cada ocorrência, fazendo com que o resultado final seja somente o último objeto declarado dentro do objeto personagens.

Apesar de prático, o uso da sintaxe de espalhamento pode gerar bastante processamento, então deve ser usado com cuidado em caso de loops ou funções recursivas.

Caso queira, temos outra explicação deste processo aqui no [artigo ES6 - Desestruturando objetos](https://www.alura.com.br/artigos/es6-desestruturando-objetos?_gl=1*1uvdg9y*_ga*OTg3OTYxNjIuMTcwMDYwOTY1Nw..*_ga_1EPWSW3PCS*MTcwNjgxMjY1My42LjEuMTcwNjgxNDM3NS4wLjAuMA..*_fplc*VDhhemV2YjdHQ0RMTjV5SmdCRDdhdkl2bWJ6QkptREN2VFolMkZNTEdmT1BrSGxpZUpLMzV6MW9EdFdsVmsya0NrTEFCS29xZWtrSG81bTd2bkxSTWJrZG9BRHYwZk9yQ3pwUEY0N0FIQ3JnYTNWak52dEF5Nk1BeGNuSmRJc2clM0QlM0Q.) presente na nossa plataforma.

Você sabia que também é possível utilizar esta sintaxe com arrays? Confira mais exemplos disso neste [Alura+](https://youtu.be/f8a-qwKC5yk).

### 8.4 CONHECENDO O JSON



![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/46e7c7e5-e04a-4f86-b45d-4a8325e32f13)



### 8.5 EXERCITANDO OS CONHECIMENTOS


#### Encontrando um Objeto


![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/0187b4a3-46e7-4424-91fc-fed27606a353)


#### Filtrando Objetos


![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/12f59be9-d618-49c8-a97c-3c9fd2e5b3fd)


#### Ordenando Objetos



Como ordenar nossa lista de clientes em ordem alfabética:

![image](https://github.com/FlavianaFXT/Js-objetos/assets/113718720/1c6c59cd-d6f9-4146-bf2a-8d827dbbc29e)











