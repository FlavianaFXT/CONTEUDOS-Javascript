# CONTEUDOS-Javascript
Repositorio destinado a resumo com os principais conceitos e principios orientadores de trabalho, aprendidos nos cursos que venho realizando na área. 


O objetivo desse resumo é auxiliar outros estudantes e utilizar como consulta em situações necessárias do cotidiano.


Conteúdos de Cursos realizados nas Seguintes Comunidades:

![image](https://github.com/FlavianaFXT/CONTEUDOS-Javascript/assets/113718720/751bbaa3-59d5-4430-9bb9-3faaeeaa6df9)

![image](https://github.com/FlavianaFXT/CONTEUDOS-Javascript/assets/113718720/d368247b-f0eb-49f9-a5a1-aa6d1f051131)





## INDICE

- [1 Lógica de programação](#1-lógica-de-programação)
- [2 TIPOS PRIMITIVOS](#2-TIPOS-PRIMITIVOS)

  
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
- [8 OBJETOS](#8-OBJETOS)
   - [8.1 O que são objetos?](#8.1-O-que-são-objetos?)
   - [8.2 Manipulação de Objetos](#8.2-Manipulação-de-Objetos)
   - [8.3 Percorrendo Objetos](#8.3-Percorrendo-Objetos)
        - [FOR...IN](#FOR...IN)
        - [METODOS DE OBJETO](#METODOS-DE-OBJETO)
        - [spread operator](#spread-operator)
   - [8.4 CONHECENDO O JSON](#8.4-CONHECENDO-O-JSON)
   - [8.5 EXERCITANDO OS CONHECIMENTOS](#8.5-EXERCITANDO-OS-CONHECIMENTOS)
        - [Encontrando um Objeto](#Encontrando-um-Objeto)
        - [Filtrando Objetos](#Filtrando-Objetos)
        - [Ordenando Objetos](#Ordenando-Objetos)
- [9 PENSANDO EM ALGORITMOS](#9-PENSANDO-EM-ALGORITMOS)
   - [9.1 Nosso primeiro problema](#9.1-Nosso-primeiro-problema)
   - [9.2 Representando algoritmos](#9.2-Representando-algoritmos)
   - [9.3 Ordenação com Selection Sort](#9.3-Ordenação-com-Selection-Sort)
      - [Usando loops do JavaScript](#Usando-loops-do-JavaScript)
   - [9.4 Insertion Sort](#9.4-Insertion-Sort)
   - [9.5 Comparando Algoritmos](#9.5-Comparando-Algoritmos)
     - [Tabelas de comparação](#Tabelas-de-comparação)
     - [Big O Notation](#Big-O-Notation)
   .................... FALTA ................................
   - [9.11 CONCLUSÃO ALGORITMOS](#9.11-CONCLUSÃO-ALGORITMOS)



  # 1 Lógica de Programação

<br/>
[1.1 O que é um algoritmo](#1.1-O-que-é-um-algoritmo)

[1.2 Linguagem de programação](#1.2-linguagem-de-programação)

[1.3 O que é Javascript](#1.3-O-que-é-Javascript)

[1.4 Console](#1.4-Console)
	[console.log(), alert(), confirm e prompt](#console.log(),-alert(),-confirm-e-prompt)

[1.5 JavaScript dentro do HTML](#1.5-JavaScript-dentro-do-HTML)
<br/>

Lógica de programação é o método usado para escrever programas que um computador entenda.

A lógica de programação parte do princípio de que praticamente todas as tarefas humanas são uma sequência ordenada de passos, que acontecem durante um tempo finito e que produzem um resultado esperado.
<br/>

### 1.1 O que é um algoritmo 
<br/>
Um algoritmo, ou programa, é um conjunto de instruções que reunimos para se chegar num objetivo. Para isso temos a entrada, o processamento (o modo de executar) e a saída. Uma maneira simples de pensarmos é em uma receita onde temos os ingredientes, o modo de fazer e o alimento pronto. Para o computador informamos algo, por exemplo o clique em um botão, o processamento, um conjunto de comandos e a saída, abertura de uma nova página.
Para escrever um programa de computador, você tem que dizer ao computador, passo a passo, exatamente o que você quer que ele faça. O computador "executa" o programa, seguindo cada etapa mecanicamente, para atingir o objetivo final.

Alguns exemplos de algoritmos que podemos citar: manual de instrução de aparelhos e funções matemáticas.
<br/>

###1.2  Linguagem de programação 
<br/>
A linguagem de programação é um método padronizado para comunicar instruções para um computador. É um conjunto de regras de sintaxes e semânticas usadas para definir um programa de computador. É uma linguagem que pode ser compreendida tanto por um ser humano como por um computador.

A linguagem de programação pode ser comparada às linguas faladas pelos seres humanos. A língua portuguesa, por exemplo, tem um conjunto de regras de sintaxe e de semântica, que uma pessoa precisa aprender para se comunicar com outra. No caso do computador, ele só entende comandos lógicos. Por exemplo ele não sabe o que é um pão, para ele pão é uma palavra que ele trata como texto. 

Existem diversos tipos de linguagem de programação, e elas podem ser classificadas em vários tipos. Um dos tipos de classificação é por nível de abstração, que pode ser baixo ou alto. As linguagens de baixo nível normalmente estão relacionadas a tarefas que acontecem na arquitetura do computador. As de alto nível as vezes precisam de um compilador (um programa intermediário que traduz o que o ser humano escreveu para uma linguagem que a máquina entenda), como Java e C.

Podemos falar “oi” em muitos idiomas. Podemos dizer “oi” em português, inglês, árabe ou japonês. São formas diferentes, mas no fim temos a mesma situação, estamos fazendo uma saudação a alguém.
<br/>

 ###1.3 O que é Javascript
<br/>
JavaScript é uma linguagem de programação interpretada (não precisa de um compilador, ela é lida diretamente pelo navegador) estruturada (ênfase em sequência, decisão e, iteração - subrotinas, laços de repetição, condicionais e, estruturas em bloco), client-side, de script em alto nível .Juntamente com HTML e CSS, o JavaScript é uma das três principais tecnologias da Internet. JavaScript surgiu em 1995 e permite páginas da Web interativas e, portanto, é uma parte essencial dos aplicativos da web. A grande maioria dos sites usa, e todos os principais navegadores têm um mecanismo JavaScript dedicado para executá-lo.

Javascript também é chamado de JS. Javascript e Java são linguagens completamente diferentes.

Os arquivos Javascript possuem a extensão .js.

Para programar e testar em javascript precisamos somente de um editor de código e um navegador.

---

<br/>

 ###1.4 Console
<br/>

#### Definição
<br/>
O console acessível através das Ferramentas de Desenvolvedor é uma interface conectada ao interpretador que vem incluso no navegador, e fica rodando “por trás dos panos” para ler e executar todo o JavaScript que o HTML contenha. O objeto Console fornece acesso ao console de depuração do navegador. O seu funcionamento específico varia de navegador para navegador, mas existe um conjunto de ferramentas que na prática são fornecidas normalmente.

Essa é uma ferramenta extremamente útil, pois ela permite que você veja erros, execute códigos em JavaScript e teste suas implementações antes de programá-las de fato em um arquivo. Aprender a ler as mensagens que o console mostra é essencial no dia a dia do desenvolvedor, visto que entender um erro, por exemplo, acelera o processo de entendimento e correção do problema de código.

Com o navegador aberto como abrir o painel dedicado Console:

- Pressione F12 ou fn+F12, se o DevTools não estiver aberto no console pressione o botão do Console.
- Pressione Ctrl+Shift+J (Windows/Linux) ou Cmd+Opt+J (Mac)
- Clique com o botão direito do mouse em uma página web qualquer e clique na opção Inspecionar/Inspect, se o DevTools não estiver aberto no console pressione o botão do Console.
<br/>


#### console.log(), alert(), confirm e prompt
<br/>
O `console.log()` é uma funcão que utilizamos para testar nosso código. O resultado será impresso no console do navegador.

```js
let mensagem = "Mensagem que vai aparecer no nosso alerta";
console.log(mensagem);
```

O `alert()` tem a mesma função do console.log, porém ele mostra uma mensagem na tela do usuário.

```js
let mensagem = "Mensagem que vai aparecer no nosso alerta";
alert(mensagem);
```

O `confirm` é um alerta que nos oferece uma lógica, com dois botões (`Ok` (true) e `Cancel` (false))

```js
let mensagem = "Aperte o botão ok";
confirm(mensagem);
// Se o usuário apertar Ok vai retornar true, se apertar Cancel vai retornar false
```

O `prompt` é um alerta que nos oferece, além da lógica de botões, um input para coletarmos variáveis.

```js
let nome = "Digite o seu nome";
prompt(nome);
```
<br/>


1.5 ### JavaScript dentro do HTML
<br/>
Você precisa avisar ao navegador que existe um arquivo Javascipt e que ele precisa carregá-lo.

```javascript
<script src="./js/index.js" defer></script>`
```

```javascript
<script>
  Seu script 
  Essa não é uma boa prática, serve apenas para estudos e testes.
</script>
```

---

<br/>

       
# 2 TIPOS PRIMITIVOS

[2.1 O que são](#2.1-O-que-são)

[2.2 Tipo Number](#2.2-Tipo-Number)
	[Operadores](#Operadores)
[2.3 Tipo String](#2.3-Tipo-String)
[2.4 Tipo Boolean](#1.3-Tipo-Boolean)



###2.1 O que são
<br/>

Tipos de dados descrevem os diferentes tipos de dados que vamos trabalhar e guardar em variáveis.
<br/>

### Dados primitivos
<br/>
Dados primitivos são aqueles que os dados não são objetos e não possuem métodos ou propriedades. São dados que são representados diretamente no nível mais baixo da linguagem de programação. Alguns dos dados primitivos mais utilizados.

<br/>

 ###2.2 Tipo Number
<br/>
é um tipo de dado utilizado para representar valores numéricos.

```javascript
1;
5;
10.5;
10000;
```
<br/>


```
// tipo Number

const meuNumero = 3;

const primeiroNumero = 1;
const segundoNumero = 2;

const operacaoMatematica = primeiroNumero + segundoNumero;

console.log(operacaoMatematica)
```


#### Operadores 
<br/>
`+`, `-`, `/`, `*`

Podemos operar com números negativos, positivos e assim por diante. Normalmente, em linguagem de programação, não estamos restritos a números inteiros, mas podemos trabalhar com números que costumamos chamar de decimais em nosso cotidiano, que têm um ponto seguido de outros números.

#### Operador de atribuição
<br/>

O operador de atribuição é o igual (=), que atribui o valor do operando à direita ao operando à esquerda. Isto é, x = y atribui o valor de y a x.

```javascript
let y = 7; // 7 é atribuído a y
let x = y; // y é atribuído a x

- += (o valor da esquerda somado ao valor da direita é resultado)
- -= (o valor da esquerda subtraido ao valor da direita é resultado)
- \*= (o valor da esquerda multiplicado ao valor da direita é resultado)
- /= (o valor da esquerda dividido ao valor da direita é resultado)

```
<br/>

#### Operadores aritméticos
<br/>

#### Adição (+)
<br/>
```javascript
let resultado = 7 + 3;
console.log(resultado); // 10
```

#### Subtração (-)
<br/>
```javascript
let resultado = 5 - 2;
console.log(resultado); // 3
```

#### Multiplicação(\*)
<br/>
```javascript
let resultado = 5 * 4;
console.log(resultado); // 20
```

#### Divisão (/)
<br/>
O operador de divisão produz o quociente de seus operandos onde o operando da esquerda é o dividendo e o da direita é o divisor.

```javascript
let resultado = 10 / 2;
console.log(resultado); // 5
```

#### Módulo (%)
<br/>
O operador módulo retorna o resto inteiro da divisão de um numero pelo outro.

```javascript
let resultado = 10 % 2;
console.log(resultado); // 0
```
#### Sintaxe simplificada:
<br/>
- Incremento (++) (Soma 1)
- Decremento (--) (Subtrai 1)
- Expoente (\*\*)
<br/>

### Operadores de comparação
<br/>

Um operador de comparação compara seus operandos e retorna um valor lógico (true ou false) baseado em se a comparação é verdadeira. Os operandos podem ser numéricos, strings, lógicos ou objetos.

<br/>

#### == Igual
<br/>
Retorna verdadeiro caso os operandos sejam iguais caso contrário retorna falso. Neste caso é apenas comparado o valor do dado e não é levado em conta o tipo.

```javascript
3 == 1; // false
3 == 3; //true
"3" == undefined; // false
3 == "3"; // true
```
<br/>

#### === Estritamente igual
<br/>
Retorna verdadeiro caso os operandos sejam iguais e do mesmo tipo.

```javascript
3 === 3; // true
3 === 3; //false
```
<br/>


#### != Não igual
<br/>
Retorna verdadeiro caso os operandos não sejam iguais.

```javascript
3 != 4; // true
3 != "3"; // false
```
<br/>

#### !== Estritamente não igual
<br/>
Retorna verdadeiro caso os operandos não sejam iguais e/ou não sejam do mesmo tipo.

```javascript
3 !== "4"; // true
3 !== "3"; // true
```
<br/>

#### > maior que
<br/>
O operador de Maior retorna true se o operando da esquerda for maior que o operando da direita.

```javascript
4 > 3; // true
```
<br/>

#### >= maior ou igual a
<br/>
O operador maior ou igual retorna true se o operando da esquerda for maior ou igual ao operando da direita.

```javascript
4 >= 3; // true
3 >= 3; // true
```
<br/>

#### < menor que
<br/>
O operador menor retorna true (verdadeiro) se o operando da esquerda for menor que o operando da direita.

```javascript
3 < 4; // verdade
```
<br/>

#### <= menor ou igual a
<br/>
O operador menor ou igual retorna true (verdadeiro) se o operando da esquerda for menor ou igual ao operando da direita.

```javascript
3 <= 4; // verdade
```
<br/>

### Operadores Lógicos
<br/>
Operadores lógicos são utilizados tipicamente com valores booleanos (lógicos - true ou false); neste caso, retornam um valor booleano. 
Entretanto, os operadores && e || na verdade retornam o valor de um dos operandos especificados, de forma que se esses operadores forem utilizados com valores não-booleanos, eles possam retornar um valor não-booleano.
<br/>

#### && E lógico
<br/>
No caso de operar expressões se o primeiro valor for verdadeiro, ou puder ser convertido pra verdadeiro retorna o segundo valor. Se o primeiro valor for falso, retorna falso.
No caso de operar apenas valores booleanos o && retorna verdadeiro apenas se ambos valores sejam verdadeiros, caso contrário retorna falso

```javascript
true && "oi"; // "oi"
"oi" && true; // true
true && false; // false
false && true; //false
true && true; //true
```
<br/>

#### || Ou lógico
<br/>
No caso de operar expressões se o primeiro valor for verdadeiro, ou puder ser convertido pra verdadeiro retorna o primeiro valor. Se o primeiro valor for falso, retorna falso.
No caso de operar apenas valores booleanos o || retorna verdadeiro se um dos valores seja verdadeiro, caso os odois valores sejam falsos retorna falso.

```javascript
false || true; // true
false || false; // false
false || "oi"; // "oi"
false || 0; // 0
```
<br/>

#### ! Não lógico
<br/>
Esse operador inverte o valor de uma expressão

Obs: Se um valor pode ser convertido para verdadeiro, este valor é chamado de truthy. Se um valor pode ser convertido para falso, este valor é chamado de falsy.

Exemplos de expressões que podem ser convertidas para falso são:

- null;
- NaN;
- 0;
- string vazia ("");
- undefined.

Todos os outros são considerados verdadeiros.

```javascript
!true; // false
!false; // true
!"Oi"; // false
!""; // true
```
<br/>

### Operador condicional (ternário)
<br/>

O operador condicional (ternário) é o único operador JavaScript que possui três operandos. Este operador é frequentemente usado como um atalho para a instrução de if else.

```
condicao ? valor1 : valor2
```
A expressão antes do ? é a condição if, se for verdadeira o primeira ação é executada, caso contrário a segunda ação, a que vem depois dos :, é executada.

```javascript
let idade = 16;

let acesso = idade > 18 ? true : false;
```

É muito útil para testes mais básicos em que se tem apenas uma única linha de código dentro do if ou do else.

```javascript
let salario = 1000;
let bonus = salario * (salario > 1000 ? 0.1 : 0.15);
```

---
<br/>

## Estrutura de decisão
<br/>

Em muitas situações precisamos tomar decisões de algo. Se o carro já está ligado não precisamos virar a chave. Se o arroz está sequinho não precisa colocar mais água. Quando o celular chega em 100% da bateria podemos tirar da tomada. Pequenas situações da vida são decisões. 
Em um programa chamamos essa verificação de estrutura de decisão. 
Seu celular está conectado na tomada e você vai checar se já acabou de carregar. A perguntar na sua mente que muitas vezes não é feita é “já chegou em 100%”?

Pensando num comando:

SE bateria é 100%
  ENTÃO
    tire o plug do celular da tomada

Observe esse SE e ENTÃO. A estrutura de decisão na programação sempre terá essa ideia do SE (caso) algo seja verdadeiro uma ação será feita.

Essa estrutura de tomada de decisão também é conhecida como condicional, onde uma condição diz que ação deve ser feita caso ela seja satisfeita ou não.
<br/>


### Expressões condicionais simples
<br/>

```javascript
// Variável booleana verdadeira
let bateria = true;

// Condição
if (bateria) {
  // Ação caso a condição seja verdadeira
  alert("Tirar celular da tomada");
}
```
<br/>


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


### 2.3 Tipo String
<br/>

é uma sequência de caracteres utilizada para representar texto.

```javascript
"Este texto é uma informação com o tipo de dado string";
"Ana Beatriz";
"1 é um número ímpar";
```
<br/>

É fundamental que o JavaScript consiga determinar qual é o tipo de dado para poder manipulá-lo. Por exemplo, para executar cálculos matemáticos, o dado armazenado na variável precisa ser um número.

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



### Métodos e ferramentas prontas do Javascript


| O que | Como | Sobre |
| --- | --- | --- |
| para transformar todas as letras em minúsculo | `.toLowerCase()` | [MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase). |
| para transformar tudo em maiúsculo | | |
| para contar quantas letras tem uma cadeia de caracteres | `.length`| [aqui](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase) |
| para retirar espaços | | |


[métodos de string do MDN (são vários)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/String#m%C3%A9todos), com a descrição de cada um.


###2.4 Tipo Boolean

é um tipo de dado lógico utilizado para representar os valores: verdadeiro ou falso, true or false.

```javascript
false;
true;
```
<br/>



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



# 3 VARIAVEIS


*VARIAVEIS* Quando um programa precisa armazenar um valor para usar futuramente, já sabemos que usamos variáveis para isso.

Variáveis são como etiquetas em que conseguimos nomear um pedacinho da memória para quando necessário eu conseguir encontrar determinada informação salva. 

Criamos variáveis para ler um valor de um usuário, guardar um dado de outro sistema ou para realizar cálculos. 
Exemplo: precisamos criar a variável number e guardar o valor 1. Seguindo a ideia acima, number é o nome de uma etiqueta.
<br/>

### 3.1 Declarando variáveis
<br/>

Criar uma variável também é chamado de declarar uma variável e para isso existem algumas regrinhas:

- não pode começar com número
- não pode conter espaços
- não pode conter caracteres especiais (com exceção do underline '\_' e do cifrão '\$')

O javascript é uma linguagem que chamamos de case sensitive, o que significa que ele diferencia caracteres maiúsculas de minúsculas. Por exemplo: nomecompleto é difrente de nomeCompleto


Existem algumas palavras que não podemos utilizar para a criação de variáveis, pois estas palavras já tem uma função específica dentro do javascript, estas palavras são conhecidas como reservadas [clique aqui para saber quais são](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Lexical_grammar#palavras-chave)

Para declarar uma variável, podemos utilizar a palavra reservada `var`, seguida do nome da variável e o valor que estamos atribuindo a ela.

```js
var meuNome = 'Patricia';
var fruta = 'Pera';
```

Nas nossas aulas vamos utilizar a palavras reservada `let` para declarar variáveis.

`let` é a versão mais moderna de `var`. A sintaxe é mesma.

```js
let meuNome = 'Patricia';
let fruta = 'Pera';
```

Referência: https://www.w3schools.com/js/js_es6.asp
<br/>

### Comentários
<br/>

Comentar o código serve para deixar mensagens importantes para você e para outro programador que vai ler seu código.

Em JavaScript você pode fazer comentários de duas formas:

- Comentário em uma linha

```js
// Comentário simples de uma linha
```

- Comentário de múltiplas linhas

```js
/* Comentário
 de múltiplas
 linhas */
```


---
<br/>



## 3.2 Var, Let e Const



`var` --> funciona basicamente em qq parte do codigo
`let` --> surgiu com o js 2015
`const` --> impede que alguem mude o valor da variavel;


### 3.3 Tipos null e undefined

#### Null
<br/>

é um tipo de dado utilizado para representar um valor nulo ou "vazio".

```javascript
null;
```

```javascript
let y = null;
console.log(y);
```
<br/>

O `null` é um tipo especial, pois pode ser traduzido como “ausência de valor” e pode ser atribuído como valor de uma variável:


```
let input = null;

if (input === null) {
 console.log('não há informação');
} else {
 console.log(input);
}
```

#### undefined
<br/>

Este tipo também representa “ausência de valor”, porém de uma outra forma: usualmente, enquanto null é um valor atribuído a uma variável que existe e foi iniciada, undefined se refere ao valor de uma variável que não foi inicializada (ou seja, não foi atribuído nenhum valor a ela).

undefined também é o valor retornado por uma função que não tem cláusula return.

embora os dois tipos sejam utilizados para sinalizar ausência de valor, os operadores de comparação do JavaScript podem ou não diferenciá-los:


```
console.log(null == undefined); // true
console.log(null === undefined); // false
```


No cotidiano é comum considerar undefined como uma ausência de valor “inesperada” (causada por um bug ou erro no código) e null como um tipo de dado que também significa ausência de valor, mas não de maneira inesperada. Por exemplo, um campo em uma tabela de um banco de dados que esteja sem dados ou uma informação solicitada que não seja obrigatória e não tenha sido preenchida pelo usuário pode ter valor null.


O javascript é uma linguagem não tipada, onde não precisamos descrever qual é o tipo de dado de uma determinada variável, ele tenta "entender/adivinhar" qual é o tipo de dado que está na variável.

---
<br/>


Nesse caso, qual seria a diferença entre os dois casos abaixo?

```
let input = null;
let input2;

console.log(input); // null
console.log(input2); // undefined
```



### 3.4 Padrão de nomes no JavaScript



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


# 4 FUNÇÕES


Funções são blocos de código que são executados quando chamados ou invocados.
#### Assinatura
Assinatura de uma função nada mais é do que os elementos que compões uma função

```javascript
function nomeDaFuncao (parametro1, parametro2) {
  return retorno
}

function somar (x, y) {
  return x + y
}

somar(2, 4) // 6

```

No exemplo acima, a função de nome somar tem dois parâmetros 'x' e 'y' e um retono de x + y.
Parâmetros são os valores que são definidos na assinatura da função e funcionam como variáveis durante a execução da mesma.

Os parâmetros são valores que vão ser substituídos por valores que serão passados no momento de invocação. 
Quando os parâmetros recebem valores no momento da execução passam a ser chamados de argumentos da função.

Os argumentos de uma função não estão limitados a strings e números. Você pode passar objetos para uma função. 

Numa função você pode ou não retornar algo. A instrução return pode ser usada para retornar o valor para uma chamada de função.
A instrução return indica que a função terminou. Qualquer código após o retorno não é executado.

Além da declaração padrão acima as funções também podem ser expressões. Neste caso as funções são atribuídas a uma variável.

```javascript

const somar = function (x, y) {
  return x + y
}

```

As expressões de função são convenientes ao passar uma função como um argumento para outra função. 


### 4.1 Invocando ou chamando funções



Para invocar funções basta utilizar o nome da função seguido de parenteses, caso a função possua parâmetros é necessário passar os argumentos também

```javascript
function somar (x, y) {
  return x + y
}

somar(2, 4) // 6

```


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



### 4.2 Arrow Function


A arrow function é uma função de seta, isso porque utiliza uma seta na sua sintaxe. Essa é uma novidade do ES6. é semelhante à expressão de função. 
Funções de seta são funções com uma sintaxe mais enxuta e elas são sempre anônimas.


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



Existe uma diferença técnica entre uma arrow function e uma função comum em relação a uma palavra reservada, o this. Mas nesse momento de início de aprendizado não convém explicá-lo com muitos detalhes.

```javascript
const somar = (x, y) => {
  return x + y
}

somar(2, 4) // 6

```

### 4.3 Função anônima


Funções anônimas são aquelas que não possuem um nome no ato de sua declaração.

```javascript
  function () {

  }
  ou
  () => {

  }
```

 ###  4.4 Callback



Callback do inglês, chamar de volta, são funções que são passadas como argumento para outras funções e chamadas dentro de outra função para execução. As callbacks podem ser do tipo síncronas ou do tipo assíncronas. Vocês podem se aprofundar nesse tópico mais pra frente, pois já um assunto mais avançado.

```javascript
function perguntarNome () {
  return prompt("Qual o seu nome?")
}

function dizerOla (callback) {
  const nome = callback();
  return `Olá ${nome}`
}

dizerOla(perguntarNome)

```

# 5 Estrutura do `if`



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


### 5.1 Estrutura if / else
<br/>

```javascript
// Variável booleana verdadeira
var bateria = false;

// Condição
if (bateria) {
  // Ação caso a condição seja verdadeira
  alert("Tirar celular da tomada");
} else {
  // Ação caso a condição seja falsa
  alert("Deixar celular carregando");
}
```
<br/>

### 5.2 Estrutura if / else if / else
<br/>

```javascript
// Variável booleana verdadeira
let hora = 8;

// Condição
if (hora <= 12) {
  // Ação caso a condição seja verdadeira
  alert("Bom dia");
} else if (hora <= 18) {
  // Ação caso a primeira condição seja falsa e a segunda verdadeira
  alert("Boa tarde");
} else {
  // Ação caso nenhuma condição seja verdadeira
  alert("Boa noite");
}
```
<br/>



### 5.3 Switch case
<br/>

Se a condição for correspondida, o programa executa as instruções asssociadas. Se múltiplos casos corresponderem o valor, o primeiro caso que corresponder é selecionado, mesmo se os casos não forem iguais entre si.

```javascript
let dia = "Segunda";

switch (dia) {
  case "Segunda":
    alert("😴");
    break;
  case "Terça":
    alert("😐");
    break;
  case "Quarta":
    alert("🙂");
    break;
  case "Quinta":
    alert("😬");
    break;
  case "Sexta":
    alert("🤪");
    break;
  case "Sábado":
    alert("😎");
    break;
  case "Domingo":
    alert("😞");
    break;
  default:
    alert("Não foi encontrada essa condição.");
}
```
<br/>


### Importância do break (switch case)
<br/>

A instrução opcional break associada com cada case garante que o programa saia da condicional switch assim que a instrução correspondente for executada e executa a instrução que segue logo após o switch. Caso break seja omitido, o programa continua a execução para a próxima instrução dentro de switch.

Se você esquecer um break então o script irá rodar a partir do caso onde o critério foi correspondido e irá rodar também o caso seguinte independentemente do critério ter sido correspondido ou não.

---
<br/>


### 5.4 **Múltiplas condições**



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


** IMPORTANTE: Ao trabalhar com múltiplas condições e else if, lembre-se sempre que cada condição e cada bloco (if, else if e else) deve representar condições excludentes entre si! Ou seja, não pode haver ambiguidade entre as condições - uma mesma condição válida tanto no if quanto no else if, por exemplo. **


# 6 Laços de repetição
<br/>

### 6.1 Estrutura de repetição
<br/>
Da mesma forma que temos que decidir coisas na nossa vida e em software também temos que repetir ações. Escrever um programa com várias linhas repetidas não é uma boa prática. 
Laços ou loops são formas de repetir instruções um determinado número de vezes sem que haja a necessidade de repetir essas instruções. Em pseudocódigo nós usamos a palavra ENQUANTO, essa palavra indicava que os passos que estivessem descritos em seguida seriam repetidos até a nossa condição se tornar falsa. Qual condição? Não conseguimos simplesmente mandar o código se repetir sozinho, para esse laço acontecer é necessário existir uma condição para avaliar se o laço vai ser executado ou não, do mesmo jeito que fazemos com o SE/SENÃO. 


Imagine que você tem 3 boletos para pagar pelo app do seu banco que estão em uma caixa “Boletos para pagar”. Depois de pago o boleto vai para a caixa “Boletos pagos”.

          ENQUANTO houver boletos na caixa “Boletos para pagar”
            entrar na tela de pagamento do app do banco
            escanear o código de barras
            confirmar os dados do pagamento
            digitar a senha
            salvar comprovante
            colocar na caixa “Boletos pagos”


Conseguiu perceber que as instruções são repetidas para cada boleto pago? Se fosse não fosse o laço de repetição teríamos que repetir as instruções as 3 vezes

        . pegar boleto 1 da caixa “Boletos para pagar”
          entrar na tela de pagamento do app do banco
          escanear o código de barras
          confirmar os dados do pagamento
          digitar a senha
          salvar comprovante
          colocar na caixa “Boletos pagos”

        . pegar boleto 2 da caixa “Boletos para pagar”
          entrar na tela de pagamento do app do banco
          escanear o código de barras
          confirmar os dados do pagamento
          digitar a senha
          salvar comprovante
          colocar na caixa “Boletos pagos”

        . pegar boleto 3 da caixa “Boletos para pagar”
          entrar na tela de pagamento do app do banco
          escanear o código de barras
          confirmar os dados do pagamento
          digitar a senha
          salvar comprovante
          colocar na caixa “Boletos pagos”


Uma das vantagens de usar laços de repetição é que se for necessário alterar uma parte do programa não será necessário alterar em vários lugares, mas somente dentro do laço.
Por exemplo, é preciso alterar de “salvar comprovante” para “enviar comprovante por e-mail”. Com o laço é necessário alterar somente em 1 ponto, sem o laço é necessário em 3.

          ENQUANTO houver boletos na caixa “Boletos para pagar”
            entrar na tela de pagamento do app do banco
            escanear o código de barras
            confirmar os dados do pagamento
            digitar a senha
            Enviar comprovante por e-mail //nova alteração
            colocar na caixa “Boletos pagos”
<br/>


<br/>
Existem algumas formas diferentes de utilizar laços em javascript
<br/>

### 6.2 while (enquanto)
<br/>

Em Javascript este 'enquanto' se torna WHILE e funciona exatamente da mesma forma que o enquanto no pseudocódigo. A sintaxe dele no javascript é a seguinte:

          while(CONDICAO){
            Código a ser repetido se a condição for verdadeira
          }


A leitura do código acima seria:

        ENQUANTO CONDIÇÃO FOR VERDADEIRA FAÇA
          Instruções a serem repetidas
        FIM do ENQUANTO


```javascript
let frio = true;

while (frio) {
  alert("Coloque um casaco");
}
```

Outro exemplo usando números:

```javascript
while (i < 10) {
  console.log("O número é " + i);
  i++;
}
```

Enquanto o valor da variável i for menor que 10, o console irá imprimir a frase "o número é i".

Ao escrever um while é importante notar que no seu código é necessário criar uma variável fora do laço para essa condição, normalmente chamamos de contador, e em algum momento a sua condição deve ser atualizada, caso contrário o seu loop se torna infinito e no nosso caso trava o navegador. O que eu quero dizer com atualizar a condição? É necessário que o nosso loop tenha um fim e para isso a nossa condição tem que se tornar falsa.
<br/>

### 6.3 for (para)
<br/>
O comando FOR é um comando completo porque contém o início, a condição e o passo de um laço de repetição. 
  - Início - onde que o laço começa
	- Condição - até onde o laço roda (condição de fim)
	- Passo - o passo para a próxima rodada

O interessante do for é que na própria estrutura dele nós já fazemos uma atualização do valor que é usado na nossa condição de fim.
A sintaxe do for no javascript é:
	
      for(inicio; fim; passo){
        Código a ser repetido enquanto o critério de fim estiver válido
      } 


```javascript
  for (let i = 0; i < 10; i++) {
    console.log(i)
  }
```




## 7 ARRAYS

[7.1 Introdução a Arrays](#7.1-Introdução-a-Arrays)
[Acessando itens de um array](#Acessando-itens-de-um-array)
[Tamanho de uma lista](#)
[Verificando que um array é um array](#)
[Como funcionam os arrays](#)
[Adicionando Elementos](#)
[Deletando Elementos](#)
[7.2 Metodos de Array](#7.2-Metodos-de-Array)
[push](#)
[pop](#)
[shift](#)
[unshift](#)
[forEach](#)
[7.3 Alterando Arrays](#7.3-Alterando-Arrays)
Dividindo com slice()
Alterando com splice()
Alterando Strings com map()
filter
find
findIndex
reduce
For in e for of
[7.4 Concatenando Arrays](#7.4-Concatenando-Arrays)
[7.5 Laços de Repetição](#7.5-Laços-de-Repetição)
Desestruturando uma lista
For Clássico
Loop infinito


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

### Estrutura de dados 
Estrutura de dados é o ramo da computação que estuda os diversos mecanismos de organização de dados para atender aos diferentes requisitos de processamento. As estruturas de dados definem a organização, métodos de acesso e opções de processamento para a informação manipulada pelo programa.

A administração e manipulação dos dados passam pelo entendimento das estruturas de dados e dos métodos que podem ser utilizados para trabalhar com esses dados.

Logo, Estrutura de Dados - ou Data Structure - é um meio de coletar e organizar informações de uma certa forma em que seja possível realizar operações com essas informações de um jeito efetivo.


### 7.1 Introdução a Arrays


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/fa089fef-beb9-4afb-8d4d-d222d50764ef)



Arrays ou listas sõ estruturas de dados ordenadas que permitem que seja possível guardar um conjunto de informações numa única variável. Cada item que compõe essa lista normalmente é chamado de elemento. Os elementos de um array no javascript tem sua posição definida por um índice que se inicia em 0.


![lista-indices](assets/lista-indices.png)


#### Acessando itens de um array


Para acessar um item de um array é muito simples, basta utilizarmos o índice da posição do item.

``` javascript
let personagens = ["Naruto", "Midoriya", "Tanjiro", "Maki"];
personagens[0] // Naruto
personagens[2] // Tanjiro
```



#### Tamanho de uma lista


É possível saber o tamanho de uma lista acessando a propriedade length

``` javascript
let personagens = ["Naruto", "Midoriya", "Tanjiro", "Maki"];
personagens.length // 4
```

#### Verificando que um array é um array


No JavaScript nós temos o comando Array.isArray(obj); que permite verificar se um objeto é um array.

```javascript
  let lista = [];
  Array.isArray(lista) // true
```

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


### 7.2 Metodos de Array


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


### push


O comando "push" pode ser usado para adicionar valores a ele. Este comando adiciona o valor no final da lista.

```javascript
const numeros = [1, 2, 3];

numeros.push(4);

console.log(numeros); // [1, 2, 3, 4]

numeros.push(5, 6);

console.log(numeros); // [1, 2, 3, 4, 5, 6]
```



### pop


O oposto do push, ele retira e retorna o último valor do vetor.
```javascript
const numeros = [1, 2, 3, 4];

numeros.pop(); // 4

console.log(numeros); // [1, 2, 3]

numeros.pop(); //3

console.log(numeros); // [1, 2]
```


### shift


O método shift() remove o primeiro elemento de um array e retorna esse elemento. Este método também muda o tamanho do array.

```javascript
const numeros = [1, 2, 3, 4];

numeros.shift(); // 1

console.log(numeros); // [2, 3, 4]

numeros.shift(); // 2

console.log(numeros); // [3, 4]
```

### unshift


O método unshift() adiciona um ou mais elementos no início de um array e retorna o número de elementos (a propriedade length) atualizado.

```javascript
const numeros = [1, 2, 3, 4];

numeros.unshift(0); // 5

console.log(numeros); // [0, 1, 2, 3, 4]

numeros.unshift(-1); // 6

console.log(numeros); // [-1, 0, 1, 2, 3, 4]
```


### forEach



O método forEach() tem o objetivo de apenas iterar um array, ou seja, percorrer todos os elementos de um array

Logo, é importante frisar: o método forEach() não retorna nada! Ou seja, ele é útil para percorrer o array original e executar algum procedimento com cada item.

```javascript
let sum = 0;
const numbers = [65, 44, 12, 4];
numbers.forEach(myFunction);

function myFunction(item) {
    sum += item;
    console.log(sum)
} // 125
```




## 7.3 Alterando Arrays


#### **Dividindo com slice()**


Esse método retorna os elementos selecionados de um array em um novo array. Essa seleção é feita a partir do index dos itens.

Obs: esse método não remove do array original os elementos selecionados!


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

Já o splice() é diferente. Ele mexe no conteúdo do array original, adicionando itens novos enquanto remove itens selecionados.

```javascript
array.splice(indice[, contagemDeDeleção[, elemento1[, ...[, elementoN]]]);
```

indice: Índice o qual deve iniciar a alterar a lista - ou seja, a partir de qual posição serão acrescentados itens, ou a partir de qual posição serão excluídos itens.

contagemDeDeleção: indicador de quantos itens devem ser removidos de um array. Se está em 0, então nenhum elemento/item deverá ser removido. É opcional.

elemento1, ..., elementoN: Os elementos que serão adicionados no array. É opcional - caso não exista, o splice apenas removerá itens.

``` javascript
const animes = ["Naruto", "Jujutsu Kaisen", "Spy X Family", "Demon Slayer"];
let removed = animes.splice(2, 0, "CDZ");
//animes é ["Naruto", "Jujutsu Kaisen", "CDZ", "Spy X Family", "Demon Slayer"]
//removed é [], nenhum elemento removido

removed = animes.splice(3, 1);
//animes é ["Naruto", "Jujutsu Kaisen", "CDZ", "Demon Slayer"]
//removed é ["mandarim"]

removed = animes.splice(2, 1, "Dragon Ball Z");
//animes é ["Naruto", "Jujutsu Kaisen", "Dragon Ball Z", "Demon Slayer"]
//removed é ["CDZ"]

removed = animes.splice(0, 2, "Haikyuu", "Jojo", "Boku no Hero");
//animes é ["Haikyuu", "Jojo", "Boku no Hero", "Dragon Ball Z", "Demon Slayer"]
//removed é ["Naruto", "Jujutsu Kaisen"]
```

** Principal diferença: o slice() não alterará o array original! Ele apenas vai retornar a você um novo array contendo a seleção passada. Por sua vez, o splice() tem o poder tanto de remover elementos, quanto de adicionar novos elementos ao array original. **


![image](https://github.com/FlavianaFXT/Curso-Javascript-Arrays/assets/113718720/d243d406-2efb-4a45-89fc-f075a1d723f7)


Em inglês, o termo splice significa "emendar" ou "juntar". Cuidado para não confundi-lo com o método slice() que abordamos na última aula, já que seus nomes são parecidos. Até o funcionamento deles é semelhante e pode causar confusão!

O primeiro parâmetro do método splice() é o índice do elemento que queremos remover. Portanto, para remover o nome de Ana, passamos o índice 1. 
O segundo parâmetro é a quantidade de itens que queremos remover a partir desse índice. Logo, para remover o nome de Ana e de Caio, informaremos o valor 2.
O método splice() aceita um terceiro parâmetro. Então, vamos colocar a string "Rodrigo".


#### **Alterando Strings com map()**

Esse talvez seja o método de manipulação de array que você mais utilizará na sua carreira como pessoa desenvolvedora.

O método map() invoca um callback passada por argumento para cada elemento do Array e devolve um novo Array como resultado.
Existe uma infinidade de coisas que podem ser feitas com o array.map(), mas talvez a mais importante e mais usada seja o mapeamento de um array e criar um novo array incluindo as informações mais relevantes do array original. E isso pode ser feito pelo uso do callback. 

Em React um caso muito comum é utilizar o map para renderizar elementos de uma lista utilizando um componente.

```javascript
const personagens = [
    {
        nome: "Eleven",
        serie: "Stranger Things"
    },
    {
        nome: "Nairóbi",
        serie: "La casa de Papel"
    },
    {
        nome: "Klaus",
        serie: "The Umbrella Academy"
    }
];

const nomes = personagens.map((item) =>{
    return item.nome
})

console.log(nomes) // ['Eleven', 'Nairóbi', 'Klaus']
```

```javascript
const personagens = [
    {
        nome: "Eleven",
        serie: "Stranger Things"
    },
    {
        nome: "Nairóbi",
        serie: "La casa de Papel"
    },
    {
        nome: "Klaus",
        serie: "The Umbrella Academy"
    }
];

const nomes = personagens.map((item, indice) =>{
    return `${indice + 1}, ${item.nome} de ${item.pais}`
})

console.log(nomes) // ['1, Eleven de Stranger Things', '2, Nairóbi de La Casa de Papel', '3, Klaus de The Umbrella Academy']

```



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

### filter


O método filter() cria um novo array com todos os elementos que passaram no teste implementado pela função fornecida. Ou seja, ele literalmente filtra os elementos de um array de acordo com uma função com uma condição passada para ele.

Sintaxe: 

``` Javascript
const newArray = arr.filter(callback)
```

**Callback:** função que é chamada e é executada. Retorna true para manter o elemento, false caso contrário, recebendo três argumentos:

- *element*: O elemento que está sendo processado no array.
- *index*: O índice do elemento atual que está sendo processado no array.
- *array*: O array para qual filter foi chamada.

```Javascript
const idades = [32, 33, 16, 40, 2, 69];

const result = idades.filter((idade) => idade > 18);

console.log(result); // [32, 33, 40, 69]
```



##### find


O método find() retorna o valor do primeiro elemento do array que satisfizer a função de teste provida. Caso contrario, undefined é retornado.

```javascript
const array1 = [5, 12, 8, 130, 44];

const found = array1.find(element => element > 10);

console.log(found);
// expected output: 12
```

##### findIndex


O método findIndex() retorna o índice no array do primeiro elemento que satisfizer a função de teste provida. Caso contrário, retorna -1, indicando que nenhum elemento passou no teste.

```javascript

const array1 = [5, 12, 8, 130, 44];

const found = array1.findIndex(element => element === 12);

console.log(found);
// expected output: 1
```


### reduce



O método reduce() executa uma função reducer (callback) para cada elemento do array, resultando num único valor de retorno.

Sintaxe: 

``` Javascript
array.reduce(callback( acumulador, valorAtual[, index[, array]] )[, valorInicial]))
```

**Callback:** função que é chamada e é executada em cada valor no array (exceto no primeiro, se nenhum valorInicial for passado); recebe quatro argumentos: 

- *acumulador*: O índice do elemento atual que está sendo processado no array. Começa a partir do index 0 se um valorInicial for fornecido. Do contrário, começa do index 1.
  
- *valor inicial*: Opcional. Valor a ser usado como o primeiro argumento da primeira chamada da função callback. Se nenhum valorInicial é fornecido, o primeiro elemento do array será usado como o valor inicial do acumulador e o valorAtual não será lido.

```Javascript
const array1 = [1, 2, 3, 4];
const reducer = (accumulator, currentValue) => accumulator + currentValue;

// 1 + 2 + 3 + 4
console.log(array1.reduce(reducer));
// expected output: 10

// 5 + 1 + 2 + 3 + 4
console.log(array1.reduce(reducer, 5));
// expected output: 15
```



### For in e for of


Além do for tradicional que foi vimos até agora, temos outros dois derivados: o for in e o for of. Esses dois tipos de for são usados para listas. Como são derivados do for, a ideia dele muda na hora de escrever a sintaxe. No "for in" nós criamos uma variável responsável por receber o valor do índice da nossa lista. Enquanto no "for of" criamos uma variável responsável por receber o valor do elemento da lista, isso de passar elemento por elemento de uma lista nós chamamos de iterar uma lista.
Abaixo nós temos a sintaxe dos dois for:

``` javascript
for(let indice in lista){ 
  Código
}

for(let elemento of lista){ 
  código
}
```

#### For in



Nesse caso, nós estamos criando uma variável responsável por assumir o valor de cada índice da nossa lista. Sendo assim, para mostrar no console cada item da nossa lista é preciso acessar elemento por elemento usando a lista[indice].
``` javascript
for(let indice in lista){ 
  console.log(lista[indice])
}
```


#### For of



Nesse caso, criamos uma variável responsável por assumir valor de cada elemento da nossa lista. Assim, para poder mostrar cada item da nossa lista no console, precisamos usar somente o próprio elemento. É comum que o nome de listas estejam no plural por serem listas de um conjunto de coisas, nesse caso o nome da variável criada para assumir o valor de cada elemento costuma ter o nome da lista no singular. Exemplo: a lista chama filmes, a variável criada no for of chama-se filme.

``` javascript
for(let elemento of lista){ 
  console.log(elemento)
}
```


## 7.4 **Concatenando Arrays**


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



## 7.5 Laços de Repetição


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


## 8 FUNÇÕES CALLBACK


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

Um objeto é uma coleção de dados e/ou funcionalidades relacionadas (que geralmente consistem em diversas variáveis e funções — que são chamadas de propriedades e métodos quando estão dentro de objetos). Vamos trabalhar com um exemplo para entender como eles são.

#### Acessando valores de um objeto

Existem duas formas de acessar um objeto: por meio da *notação de ponto (dot notation)* ou da *notação de colchetes (bracket notation)*:

```Javascript
//notação de ponto

  pessoa.nome // Ana
  pessoa.animesFavoritos // ['CDZ', 'Naruto']

//notação de colchetes

  pessoa["nome"] // Ana
  pessoa['idade'] // 26

```

#### Adicionando propriedades a um objeto
Para adicionar uma nova propriedade a um objeto já existente podemos utilizar a seguinte sintaxe:

```javascript
let pessoa = {
  nome: "Ana"
}

pessoa.sobrenome = "Morita"

```

#### Deletando propriedades de um objeto
A palavra-chave "delete" remove propriedades específicas. Tentar ler uma propriedade inexistente terá como valor "undefined".

```javascript 
  let pessoa = {
    nome: "Ana"
  }

  delete pessoa.nome
```
### Escopo
É o contexto atual de execução, em que valores e expressões são "visíveis" ou podem ser referenciadas. Se uma variável ou outra expressão não estiver "no escopo atual", então não está disponível para uso. Os escopos também podem ser em camadas em uma hierarquia, de modo que os escopos filhos tenham acesso aos escopos pais, mas não vice-versa.

O escopo de uma função é a função na qual ela é declarada, ou todo o programa se ela é declarada no nível superior.

As variáveis definidas no interior de uma função não podem ser acessadas de nenhum lugar fora da função, porque a variável está definida apenas no escopo da função. No entanto, uma função pode acessar todas variáveis e funções definida fora do escopo onde ela está definida. Em outras palavras, a função definida no escopo global pode acessar todas as variáveis definidas no escopo global. A função definida dentro de outra função também pode acessar todas as variáveis definidas na função hospedeira e outras variáveis ao qual a função hospedeira tem acesso.


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


## 9 PENSANDO EM ALGORITMOS


## 9.1 Nosso primeiro problema

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/c666dbe2-76e0-4193-ae60-d50492b02f9c)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/9a2c35b5-7633-49bc-a1f5-487a405ebfe3)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/2d86ac09-9168-4a31-b4e3-610ee12b8c2f)


 ### Do papel para o codigo

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/32cd41c2-bf06-4734-936a-aa006af64984)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/0ceed190-0eed-4dc4-93d7-ddc943b883ba)


executa no terminal


 ### Exibindo os Livros

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/58ab0e13-0e1e-4330-89a9-89367835a178)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/9266153a-7b43-4cbc-933d-7e4728528987)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/cbfcfadd-0bc6-42e0-af5f-960363c3c3fd)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/ef30df9f-8f7b-448b-a6c8-e84da31160cf)


### 9.2 Representando algoritmos


Você já viu ou já ouviu falar de fluxogramas?

Um fluxograma é uma forma de representarmos os passos de um algoritmo, através de símbolos bem definidos para cada tipo de processo (entrada de dados, processamento, condicionais, etc) para facilitar a visualização e o mapeamento de todos os passos necessários e/ou possíveis em um determinado processo. São muito utilizados para descrever algoritmos, mas podem ser utilizados em qualquer situação que envolva um fluxo finito de ações, com entrada e saída.

Há outras formas de se representar um algoritmo além do fluxograma, como a descrição textual/verbal dos passos (que estamos utilizando nesse curso), o pseudo-código ou mesmo a própria leitura do código em JavaScript ou outra linguagem de programação. Você pode conferir exemplos destas três formas neste [artigo da Alura](https://www.alura.com.br/artigos/algoritmos-e-logica-de-programacao?_gl=1*1jqdmd2*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwODQ1NjIyMi4yOS4xLjE3MDg0NTgwNTUuMC4wLjA.*_fplc*cCUyQlRzVjZIOUVHTURUMGc3NGdOaSUyRmMwTWltSVlqJTJGRlR2ZjdKN0owMmsxQ09PdGxCZFFaS1RTa3NXWjhDN251YmRzU2RqJTJGTkZrM1NrQnd0eVhraVRWcVlDRVFlbmpSU3I2SktPUE5nN0NqZjRQUldqVjhENlM1dGQwOGZYUmclM0QlM0Q.).

No caso do fluxograma, os diferentes formatos das caixas de texto ajudam a definir os passos lógicos de um processo. Veja alguns exemplos:

Temos a representação de cinco imagens que, respectivamente, representam as figuras padrão para os tipos de operação em um fluxograma. No 1 temos uma figura com o texto início e fim, no 2 temos uma outra figura diferente, com o texto entrada (input) manual, no 3 temos uma outra imagem com a palavra processamento, no 4 temos um losango com a palavra decisão, e, por fim, na quinta e útlima imagem temos o texto entrada/saída (input/output)

As figuras padrão para os tipos de operação em um fluxograma são:

Início/fim: Marcam o início ou término do processamento que está sendo descrito, normalmente “início” ou “fim”, mas também podem ser utilizados as saídas de processamentos anteriores ou entradas de processamentos posteriores, como “envio do formulário”. Representado por uma figura oval ou retângulo com bordas arredondadas;
Entrada manual: input (ou entrada) manual de dados, por exemplo dados informados pelo usuário do sistema. Representado por um retângulo com o lado direito mais alto;
Processamento: bloco ou conjunto de operações que serão efetuadas com os dados recebidos. Representado por um retângulo;
Decisão: quando o programa pode seguir em mais de um caminho, que envolve uma decisão cujo resultado é “sim” ou “não” (os equivalentes a true e false). Representado por um losango;
Entrada/saída: Processo de recebimento dos dados pelo programa (input ) ou retorno do resultado de um processamento (output). Representado por um paralelogramo.
Vamos ilustrar melhor com um exemplo de fluxograma para uma soma entre dois números:

Temos um fluxograma vertical que se inicia com um retângulo com bordas arredondadas com a inscrição início, uma seta apontada para baixo, um retângulo com o lado direito mais alto com a inscrição num1, uma outra seta apontada para baixo. um retângulo com o lado direito mais alto com a inscrição num2, mais uma seta para baixo, um retângulo com a inscrição soma = num1 + num2, mais uma seta apontada para baixo, uma imagem com cinco lados com a inscrição soma e, por fim, uma última seta apontada para baixo seguida de umretângulo com bordas arredondadas com a inscrição fim

O fluxograma acima descreve:

o ponto de início do processamento;
a entrada de dois dados (as variáveis num1 e num2), cada um por vez;
o processamento (operação matemática entre os dois números);
a saída do resultado através da variável soma;
o fim do processamento.

Podemos representar o algoritmo acima com código JavaScript:

```
const num1 = 2;
const num2 = 2;

const soma = num1 + num2;

console.log(soma)
```


Vamos ver mais um exemplo, para um loop que exibe no console números de 0 a 10:

Temos um fluxograma que se inicia com um retângulo com bordas arredondadas com a inscrição início, em seguida, uma seta apontada para baixo e um paralelogramo com a inscrição i = 0, em seguida, temos outra seta apontada para baixo, com um losango com a inscrição i <= 10?, o fluxograma, então, se desmembra em duas ramificações. Na esquerda do losango, temos uma seta, a inscrição “não”, que leva a um retângulo com bordas arredondadas com a inscrição fim, já abaixo do losango, em outra ramificação possível, temos uma seta apontada para baixo, a inscrição “sim” e um paralelogramo com a inscrição imprime i, após esse paralelogramo, temos uma seta à direita que leva a um retângulo com a inscrição i = i + 1 e, em seguida, uma seta apontada retornando para o losango com a inscrição i <= 10?

O fluxograma acima pode ser traduzido, em código JavaScript, em um for:

```
for (let i = 0; i <= 10; i++) {
 console.log(i);
}
```


Existem outros símbolos que usamos nos fluxogramas para ilustrar outros tipos de operações possíveis, como impressão em papel ou envio de dados para um banco.

Você pode praticar com fluxogramas para criar algoritmos tanto para códigos que você já escreveu quanto para “colocar no papel” e ajudar a organizar a estrutura para um algoritmo que esteja desenvolvendo; ou mesmo treinar com outras situações, como fazer um bolo ou pagar uma conta de luz.


### Encontrar o livro mais caro


Durante a aula, criamos um algoritmo para encontrar o menor valor em uma lista (array). Mas a mesma lógica pode ser invertida para funcionar com o maior valor.

Dentro do for, basta invertermos a condição do if, para ao invés de verificar se o produto atual tem valor menor <, agora verifique se tem valor maior >:

```
let maisCaro = 0;
for (let atual = 0; atual < livros.length; atual++) {
 if (livros[atual].preco > livros[maisCaro].preco) {
   maisCaro = atual;
 }
}
```


Futuramente este loop poderá ser extraído para uma função que faz ambas as operações e consegue, com o mesmo código, encontrar tanto o valor menor quanto o maior.


### 9.3. Ordenação com Selection Sort


#### Ordenar para organizar


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/1188de6f-8dbe-40ab-b50f-09e59ad4814c)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/dfdf79c2-d757-41b0-90f0-e3b9852b2ebd)


#### Selection Sort

Ordenação por seleção

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/1bcdf6bd-298b-4aa3-9ca1-441c202c8109)



#### O sort() do JavaScript


Durante este curso estamos criando nossos próprios algoritmos de busca e ordenação. Porém, se formos investigar a documentação do JavaScript, descobrimos que o pacote da linguagem já traz, prontos para uso, métodos/funções que buscam ocorrências e ordenam listas, da mesma forma que estamos fazendo. Por exemplo, para varrer arrays em busca de dados específicos, podemos utilizar includes(), find() ou filter(), entre outros, e para ordenar arrays podemos usar o método sort().

Mais do que pensar “por que não usamos o método pronto do JavaScript ao invés de escrever outro do zero?” vamos olhar por outro ângulo: se o JavaScript tem um método/função de ordenação “pronto para usar”, esse método com certeza utiliza algum algoritmo de ordenação para fazer esse trabalho. E qual seria ele? É o mesmo que utilizamos?

A verdade é que o sort() utiliza mais de um algoritmo de ordenação, dependendo de principalmente duas coisas: 1) as características do array a ser ordenado e 2) a implementação do JavaScript que está sendo utilizada.

Como assim, implementação?

O JavaScript se desenvolveu como uma linguagem interpretada pelos navegadores, e a partir da especificação do que cada versão da linguagem deve seguir (definida pelo [ECMA](https://ecma-international.org/publications-and-standards/standards/ecma-262/) cada navegador implementa os métodos e funções de acordo com suas próprias engines, ou seja, cada navegador tem seu próprio “motor” de interpretação do JavaScript, e a forma como o código é interpretado “por baixo dos panos” em cada navegador pode ser diferente.

No caso do método sort(), a engine de interpretação do JavaScript implementada pela Mozilla no navegador Firefox utiliza um algoritmo chamado Merge Sort, enquanto o Google utiliza, na engine do Chrome (chamada de V8) alterna entre outros dois algoritmos de ordenação, o Quick Sort e o Insertion Sort, dependendo do caso. Existem vários algoritmos de ordenação!

No caso do NodeJS, uma vez que utiliza como base a engine V8 do Google, os algoritmos utilizados no sort() também serão os mesmos.

E que casos são estes? O método sort(), executado sem nenhum parâmetro, interpreta todos os elementos do array como strings e ordena em ordem alfabética crescente, a partir da tabela [Unicode](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Grammar_and_types). Para outros tipos de ordenação, por exemplo numérica ou decrescente, é preciso passar parâmetros de comparação para o sort().

A [documentação do MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/sort) sobre o sort() tem vários exemplos sobre os diversos casos de ordenação e como utilizar este método.


#### Usando loops do JavaScript


Durante o curso vamos usar o for para escrever os laços de repetição. Esta forma de escrever laços é muito comum em linguagens de programação e pode ser encontrada praticamente da mesma forma tanto no JavaScript quanto em outras linguagens muito utilizadas, como o Java e a família C (C, C++, C#, entre outras). Assim como o for, a maior parte dessas linguagens, além de várias outras, também utiliza os laços while e do… while.

O JavaScript tem outras formas de escrever laços de repetição além desse for “clássico” e podemos reescrever o nosso código para testar com um método mais moderno, o forEach().

forEach() é um [método de array](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach) do JavaScript que percorre o array e executa um bloco de código para cada índice.

Este método pede como parâmetro uma função que chamamos de função callback. Esta função callback controla o laço para que percorra cada um dos elementos do array, através do parâmetro que estamos chamando de livro (afinal de contas, trata-se de um array de livros):

```
livros.forEach((livro) => {
  // código aqui
})
```

Também vamos precisar do número do índice de cada elemento, para fazer a troca de lugares entre os valores. Para isso vamos precisar do segundo parâmetro da função callback, que é opcional, e que leva justamente o número do índice atual que está sendo percorrido. Ou seja, é o equivalente à nossa variável atual:

```
livros.forEach((livro, indice) => {
  // código aqui
})
```

Agora podemos passar para dentro do bloco a lógica do algoritmo, substituindo atual por indice:

```
livros.forEach((livro, indice) => {
 let menor = menorValor(livros, indice)

 let livroAtual = livros[indice];
 let livroMenorPreco = livros[menor];

 livros[indice] = livroMenorPreco
 livros[menor] = livroAtual 
})
```

Se examinarmos o laço, vemos que o primeiro parâmetro da função callback, livro, não está sendo utilizado; nesse caso, podemos usar a notação do JavaScript para informar que o primeiro parâmetro não será utilizado no código, através do _:

```
livros.forEach((_, indice) => {
 let menor = menorValor(livros, indice)

 let livroAtual = livros[indice];
 let livroMenorPreco = livros[menor];

 livros[indice] = livroMenorPreco
 livros[menor] = livroAtual 
})

console.log(livros)
```


Agora é só testar com node selectionSort.js.


### 9.4 Insertion Sort


um novo algoritmo (Insertion Sort) para resolver o mesmo problema do algoritmo anterior (Selection Sort); ou seja, ambos são algoritmos de ordenação.


#### Outras formas de Ordenar

Ordenação em ordem alfabética.


#### Programando o algoritmo

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/4659444d-bb0e-40bf-9cb8-7ac1831f4883)


#### Mais testes de Mesa - Desk Checking

interpretar o código passo a passo, anotando o que tem dentro de cada variável, em cada momento de cada linha de cada passo do loop.

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/409d013e-2ff8-4fa7-8e59-c0b8aadb2b1c)

Um teste de mesa é justamente o processo manual de verificar todas as linhas de um código e executá-lo passo a passo com ajuda de, por exemplo, papel e lápis para anotar qual os valores das variáveis em cada passo de cada linha. É como compilar/interpretar um bloco de código usando o cérebro como compilador/interpretador.

Apesar de hoje as [IDEs](https://www.alura.com.br/artigos/o-que-e-uma-ide?_gl=1*1wv7q5s*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwODYwNTg5OC4zMS4xLjE3MDg2MDgxMTQuMC4wLjA.*_fplc*YlZBS01jN2t3RFd2ZEZNSzFicEpscEtDRHVQSW5GZ0g4akI0ZWFlRFVTNyUyQlhpSzU3U0MxdlBlak9iZDJQTzQ3MzlPWXpqVVIyNEwyM2pCdDU0QmVEdHQ5S2t0M2VzJTJCVW5temNsczhsU21JU2hpZGx4TWQ5QUtHdEJnbmVRZyUzRCUzRA..) e as linguagens terem ferramentas práticas, modernas e eficientes para avisar, “debugar” e encontrar erros de código, o teste de mesa é uma forma muito boa de se estudar lógica de programação e para entender o que acontece em cada passo de execução do código, especialmente no caso de algoritmos que envolvem laços de repetição, substituição de valores e variáveis temporárias, como vimos durante a aula.

Uma forma muito comum de fazer o registro de valores de variáveis durante um teste de mesa é utilizando tabelas de rastreio, ou trace tables. Por exemplo, um teste de mesa para um for que imprime números de 0 a 5 no console poderia ser representado pelo seguinte teste de mesa/tabela de rastreio:

Captura de tela do editor de código mostrando um trecho de código e, à esquerda, o número de cada linha. Na linha 1: let num = 0; na linha 2: console.log(num); na linha 3 não há código; na linha 4: for (let i = 1; i <= 5; i++) {; na linha 5: console.log(i); na linha 6: } (fechamento de bloco).

```
linha	num	i	saída
1	0		
2			0
4		1	
5			1
4		2	
5			2
4		3	
5			3
4		4	
5			4
4		5	
5			5
4		6
```


Nos seus exercícios e testes, a tabela pode tranquilamente ser feita com papel e lápis, se preferir.

O importante no teste de mesa (com ou sem uso da tabela) é percorrer cada linha e executar realmente o código, anotando as criações/reatribuições de variáveis, resultados de operações matemáticas (se houver), alterações em arrays e objetos, etc. Dessa forma, resultados não esperados na execução do código já vão aparecer na hora.



#### Extraindo funções


Durante a aula, utilizamos duas vezes a seguinte estrutura de código:


```
let itemAnalise = lista[analise];
let itemAnterior = lista[analise - 1];

lista[analise] = itemAnterior
lista[analise - 1] = itemAnalise
```


Repetição de código quase sempre é sinal de que o trecho repetido poderia ser extraído para uma função, assim pode ser reaproveitado. Vamos ver como podemos fazer isso:

Vamos começar criando um novo arquivo, que vamos chamar de troca.js, e dentro dele a função:

```
function troca(lista, analise) {
  // código aqui
}
```


A função troca() vai fazer toda a lógica de substituição de valores dentro de insertionSort(), então vamos trazer de lá o código correspondente e ver o que precisamos refatorar:

```
function troca(lista, analise) {
 let itemAnalise = lista[analise];
 let itemAnterior = lista[analise - 1];

 lista[analise] = itemAnterior
 lista[analise - 1] = itemAnalise
}
```


Veja que a função troca() está fazendo alterações direto na lista que está sendo passada por parâmetro; assim, essa função não precisa retornar nenhum valor.

Sem esquecer de exportar a função no final do arquivo, para que possamos importá-la em insertionSort.js:

```
function troca(lista, analise) {
 let itemAnalise = lista[analise];
 let itemAnterior = lista[analise - 1];

 lista[analise] = itemAnterior;
 lista[analise - 1] = itemAnalise;
}

module.exports = troca;
````

Agora, no arquivo insertionSort.js, começamos importando a função troca() no topo do arquivo:

```
const troca = require('./troca');
```

E todo o trecho que foi passado para a função troca() pode ser substituído pela chamada da função:


```
function insertionSort(lista) {
 for (let atual = 0; atual < lista.length; atual++) {
   let analise = atual;
   while (analise > 0 && lista[analise].preco < lista[analise - 1].preco) {
     troca(lista, analise);
     analise--
   }
 }
 console.log(lista);
}
```


Veja que estamos passando como parâmetro da função troca() o array que vamos trabalhar (lista, o mesmo parâmetro que passamos como parâmetro da função externa, insertionSort()) e a variável analise. Dessa forma, a cada laço de repetição feito com o for, de 0 ao fim do array, o valor da variável analise também será atualizado, e este novo valor é passado como parâmetro da função troca() também a cada laço.



## 9.5 Comparando Algoritmos


*Complexidade do selection sort*

Vamos começar analisando os algoritmos que nós criamos para fazer uma busca pelo menor número, nós chamamos essa função de menorValor. Então, vamos ver como nós analisamos, em termos de processamento, esse algoritmo de busca que acabamos criando.

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/ba733e32-fb6d-494b-a41d-2657bdd71fb8)

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/2d4d3ad2-bdab-49b2-b1f2-0e6a1f4f2943)


*Comparando com Numeros*



Já estamos desenhando de cabeça qual é o processo de descobrir a complexidade de um algoritmo, mas é sempre mais legal trabalharmos com números para termos uma ideia melhor.
Como fizemos anteriormente com o nosso algoritmo buscaMenor, vamos deixar a planilha de Excel calcular para nós a quantidade de operações dada uma quantidade n de elementos em uma lista.

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/dab2138c-2d02-4aa6-ac77-fbe3cfbe82b5)

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/1df4ccc4-7f87-4db4-a9d8-13f7e93b2a32)



*Simulando um computador*



Você já prestou atenção nas informações técnicas de um computador? Quando vamos comprar um computador, o que significam alguns daqueles números de processador, de velocidade etc., e o que isso tem a ver com os cálculos que estamos fazendo aqui, que estamos até utilizando a planilha, já saímos do código.
O que vamos fazer é ver de uma forma um pouco mais simplificada como que a quantidade de operações que estamos calculando na nossa planilha impacta no processamento do computador, em como o computador processa essas informações.


A complexidade de um algoritmo impacta diretamente no seu processamento, já que a memória do nosso computador não é infinita.


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/1f833ca9-0cd9-4551-b849-f92f53e0a4f1)


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/24abe043-5f66-4b84-986c-9ac76d4c6d01)


vídeo nesse [link](https://www.youtube.com/watch?v=BeoCbJPuvSE&feature=youtu.be)! Veja como existem vários outros algoritmos apenas para resolver o problema de ordenar listas, como Quick Sort, Radix Sort e etc. Todos esses algoritmos já foram desenvolvidos anteriormente, assim como o Selection Sort e o Insertion Sort que utilizamos durante o curso.

Se quiser checar outros modos de visualizar os dados, pode buscar por sorting algorithm comparison no YouTube e comparar os resultados.

Você pode praticar a implementação em javaScript de alguns desses outros algoritmos!


#### Como funciona um processador


Nesta aula falamos muito brevemente sobre como funciona um processador, e simplificamos um pouco o tema para trabalhar com nossos exemplos.

É interessante que você, ao começar seus estudos em programação, busque também relacionar o código e a forma como ele é interpretado pelo computador. Esse conhecimento nos ajuda a entender o porquê de alguns comportamentos das linguagens de programação, porque alguns bugs acontecem e como corrigi-los ou evitá-los. E, como vimos durante a aula, essa questão pode ser essencial para uma boa performance dos nossos programas.

Para entender melhor como o computador processa as informações e o que significam alguns dos números e siglas que acompanham os modelos dos componentes de computadores, você pode conferir o nosso curso de Arquitetura de computadores.


#### Tabelas de comparação


Utilizamos o Google Sheets (equivalente ao Excel) para montar as tabelas de comparação de algoritmos.

Caso queira replicar as tabelas e fazer mais testes, pode aproveitar as fórmulas que usamos na aula:


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/5336af85-17b0-437a-8425-08063ecee42a)


```
elementos	n	2n	n^2	2*n^2	1	n^3
1	=+A2	=2*A2	=A2*A2	=2*D2	1	=A2A2A2
=+A2*2	=+A3	=2*A3	=A3*A3	=2*D3	1	=A3A3A3
=+A3*2	=+A4	=2*A4	=A4*A4	=2*D4	1	=A4A4A4
=+A4*2	=+A5	=2*A5	=A5*A5	=2*D5	1	=A5A5A5
=+A5*2	=+A6	=2*A6	=A6*A6	=2*D6	1	=A6A6A6
```

A tabela acima está preparada para uma lista de até 16 elementos, mas você pode expandir a partir daí e ver os resultados!


#### Outros tipos de Algoritmo


Voltando à planilha e aos gráficos que estávamos gerando, nós comparamos o crescimento de um algoritmo linear com um algoritmo quadrático anteriormente, mas será que existe algum algoritmo que seja mais rápido do que o linear?

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/641851df-0a2a-43a7-bf91-4c5db24e4f58)

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/4b93673e-46fd-4ed9-98e1-410ae693c55a)

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/fec5ddb5-f582-4e3b-a722-a95951d2b449)

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/8075900c-360d-4f37-9e0e-40b015be36f5) Bugou o grafico


 normalmente, no dia a dia, nós não trabalhamos com uma lista de 128 elementos, trabalhamos com quantidades muito maiores de dados.
 Por isso, sempre temos que saber: como analisamos algoritmos, que eles precisam ser analisados com relação à complexidade deles; tem que levar o índice de crescimento em conta – se é quadrático, se é linear, se é logarítmica etc.
Que existem vários tipos de crescimento e vários algoritmos prontos - selectionSort e insertionSort são só dois deles para ordenação, porque existem algoritmos para todos os tipos de problema; e cada um tem as suas vantagens e desvantagens.


#### Big O Notation


Ao começarmos o estudo de algoritmos, é comum nos depararmos com a expressão Big O Notation (ou Notação “O Grande”).

Essa notação é utilizada para expressar a complexidade de um algoritmo, com relação ao tempo e volume de recursos computacionais necessários para executar esse algoritmo, de acordo com o volume de dados de entrada. Em geral, utiliza-se o tempo de uso de CPU (unidade central de processamento) do computador.

Ou seja, usamos O para classificar funções (implementações de algoritmos) de acordo com a forma como crescem em complexidade. Algoritmos diferentes podem crescer em complexidade da mesma forma, então podem ter a mesma classificação O, como vimos durante o curso com o Selection Sort e o Insertion Sort.

Podemos classificar os exemplos que vimos durante a aula da seguinte forma:


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/583eabf3-323c-4f6f-b319-cb4207b2a9d1)


A função menorValor() é um exemplo de algoritmo de crescimento linear: o “custo” (referente à quantidade total de operações necessárias) depende da quantidade de elementos na lista; uma lista de 10 elementos resulta em 10 operações de busca e uma lista de 1000 elementos resulta em 1000 operações. Ou seja, menorValor() tem complexidade de O(n), onde n é o tamanho (quantidade de elementos) da lista.

Já nas funções selectionSort() e insertionSort(), vimos que um laço de repetição dentro do outro faz com que a taxa de crescimento não aumenta mais de forma linear com relação à quantidade de elementos na lista, porém de forma quadrática, pois um laço dentro de outro significa que a quantidade de operações será de n*n (sendo n a quantidade de elementos). Ou seja, selectionSort() e insertionSort() têm complexidade de O(n²).

Como os exemplos que vimos na planilha e nos gráficos da aula, existem outras formas de avaliar o crescimento de um algoritmo, e que também podem ser representada segundo a notação O grande:


![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/8efa9c44-b710-4e18-8c08-ecef785f6bda)


A notação O grande não é usada apenas em computação, mas também em várias áreas da matemática e existem outras notações na lista além dos exemplos que utilizamos.

Se quiser saber mais e ter outros exemplos de notações relacionadas a algoritmos comuns em programação, o site [Big O cheatsheet](https://www.bigocheatsheet.com/) (em inglês) fornece ótimo material para estudo.


*Mais cálculos de complexidade*


Podemos aproveitar a planilha e os gráficos que utilizamos na aula para testar a complexidade (pela notação O grande) de outros algoritmos, como a logarítmica e a linear-logarítmica, além das que vimos na aula:

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/b5b0e413-7ff4-4bd4-8a8d-220518464dc3)

Se quiser fazer mais testes, atualize sua planilha com as fórmulas que utilizamos e expanda para maiores quantidades de elementos:

![image](https://github.com/FlavianaFXT/Js-algoritmos-de-ordenacao/assets/113718720/7f798970-fa65-448d-82da-53c71065865e)

Atualize os gráficos e veja os resultados!


### 9.6 DIVIDIR PARA CONQUISTAR


#### Misturando Listas

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/005b8f86-a53f-4cb3-b997-c7f27cefb348)

Esse tipo de simulação que fazemos em código já vimos que nos ajuda bastante a entender como funciona o fluxo, os passos de um algoritmo, por exemplo, de ordenação, antes de tentarmos fazer o código dele.


#### Testando o Algoritmo

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/d31d5fbb-1226-4bbc-bbfc-c9c2e7bfbebb)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/2c0716dc-9ba5-485b-9faf-2f01a8ae4f82)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/05df785c-ad6a-4ee2-841a-814b490168be)


#### Passando para o código

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/072a4f05-b66f-42bd-95b4-e8d704c16f73)



### 9.7 MERGE SORT


#### Intercalando Valores

O Merge Sort pega duas partes de um todo, separa, compara e depois funde. a gente pega um problema grande, divide em partes pequenas para resolver melhor o todo.

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/79fa9ae5-6e80-43bd-9096-fcee3923ecfd)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/3b98a37c-028c-4401-a9dd-443255ed6e4a)


#### Como o Merge Sort funciona

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/da42e16c-b3d5-44d3-a0d5-86da507285c9)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/9f20de16-446b-4a8a-a0a8-cfe9fba22ec6)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/3bd189c7-56f2-4f60-b05f-776416bbdbec)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/eeefabd7-2b04-4b6f-b312-a393ab59e039)

Entendendo o que precisamos fazer, vamos passar isso pro codigo.


#### Implementando o Algoritmo


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/6a7544d4-8fa5-4f6b-89c2-763c10418e48)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/d6436f6b-4b29-4ff7-b2e1-956a49b0a7c3)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/7cb6ccde-1d0b-4708-a7e6-e2995ead0f60)


#### Recursão


Vamos revisar o que aconteceu na nossa função mergeSort, para ficar bem claro como a recursão está funcionando.

Recursão é basicamente resolver um problema em partes menores até que tenhamos resolvido o problema completo. É uma forma parecida com a lógica que está por trás do próprio merge sort.

Muitas vezes isso envolve uma função ficar chamando ela mesma até que isso não seja mais necessário.

 Parece um pouco com laço de repetição, mas a execução é bem diferente.

Revisitando então a nossa função mergeSort, a primeira linha dentro dessa função é uma condição que só vai executar o código que está dentro do mergeSort se o array que for passado por parâmetro for de um tamanho maior do que 1.

Se não for, simplesmente retorna aquele único elemento, que é o que vimos nas simulações inclusive. Se só temos um elemento, não tem o que dividir nem o que comparar, só retorna ele.

E como o código faz isso? Ele faz, através do trecho onde ele pega o valor da metade do array e usa esses valores para dividir, para fazer um slice. E a cada vez que mergeSort é chamado, o array que é passado por parâmetro para dentro dele é um array cada vez mais dividido, cada vez menor. E é aqui que a recursão está sendo executada.

 Cada vez que o array é dividido, mergeSort é executado novamente, recebendo um array cada vez menor por parâmetro, até que a condição desse if não seja mais atendida.

Nesse momento em que a condição do if não é mais atendida, o mergeSort para de ser chamado na primeira chamada recursiva que estamos fazendo, e o resultado será retornado e guardado dentro da constante parte 1.

A mesma coisa se dá para a parte 2. Isso é executado até que não atenda mais a condição do if. Quando isso acontece para de ser feita a chamada recursiva de mergeSort, e o resultado é guardado dentro da variável parte 2.

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/43fc76ed-88c3-488f-a8d0-be8a1dcb282f)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/27defa8a-839c-46e1-9690-13b1001090ba)


Quando pesquisamos sobre recursão, normalmente encontramos duas definições que se completam:

1) Um método utilizado para resolver problemas de computação em que a resolução consiste em solucionar instâncias menores do mesmo problema;

2) Um método em que uma função ou algoritmo chama a si uma ou mais vezes até que se atinja uma condição específica, quando o resultado de cada repetição é processado desde a última chamada até a primeira.

Um exemplo interessante de código para ilustrar esse cenário seria o seguinte:

Abaixo é definida uma função para controlar a frequência com que os números são incrementados durante a execução da função recursiva incrementaNumero(), que será definida a seguir:


```
function dorme(milissegundos){
        return new Promise(resolve => setTimeout(resolve, milissegundos));
}
```


Aqui é definida uma função assíncrona recursiva que incrementa o número passado como parâmetro em uma unidade e, após 2 segundos, chama a si própria antes de encerrar a sua execução, ilustrando efetivamente um caso de recursão:


```
async function incrementaNumero(numero){
  console.log(numero)
  await dorme(2000)
  return incrementaNumero(numero + 1)
}

incrementaNumero(1)
```


Para o qual a saída seria:

```
1
2
3
4
5
```

Como podemos ver, a função incrementa o número passado como parâmetro em uma unidade e, antes de sair, chama a si própria novamente.

Ainda que o exemplo passado seja uma forma bastante objetiva de demonstrar recursividade, a sua utilização no mundo real não é muito prática já que essa função continuaria realizando o mesmo processo infinitamente - não foi passada nenhuma condição de saída - e não seríamos capazes de retirar valor da sua execução.

Para solucionar esse problema existem os base cases ou, em português, casos base. Mas o que são esses casos base? São uma forma de passar para a função uma condição de controle para a recursividade ou, em outras palavras, uma condição de saída.

Segue exemplo de caso base para função recursiva:

Abaixo é definida uma função para controlar a frequência com que os números são incrementados durante a execução da função recursiva incrementaNumero() que será definida a seguir:

```
function dorme(milissegundos) {
  return new Promise(resolve => setTimeout(resolve, milissegundos));
}
```


Aqui é implementada uma função recursiva com caso base:


```
async function incrementaNumero(numero){
  console.log(numero)
  await dorme(2000)
```


Aqui é implementada o caso base(base case) que fará com que a função pare a recursão quando o valor do parâmetro numero for igual a 10:


```
async function incrementaNumero(numero){
  console.log(numero)
  await dorme(2000)

  if (numero === 10) {
          return 'finalizou'
  }
  return incrementaNumero(numero + 1)
}

incrementaNumero(1)
```


A saída então será:

```
1
2
3
4
5
6
7
8
9
10
```


É importante lembrar que a função recursiva é aquela que chama a si mesma até encontrar uma condição de saída/parada. A recursividade é uma técnica muito aplicada em estruturas de dados, algoritmos e gráficos.

Por exemplo, é recursão o efeito de tela infinita que surge em suas chamadas de vídeo ou quando você coloca um espelho em frente ao outro. No entanto, temos a possibilidade e obrigação de inserir uma verificação que interrompa este comportamento, ou então a função entrará em loop infinito.


#### Além do console.log()


Acredite ou não, o objeto console do nosso amigo JavaScript tem muito mais métodos do que o log().

Ele também conta com um método chamado trace() que, além de imprimir mensagens, também fornece um stack trace, uma espécie de rastro de execução das funções executadas.

De forma bem simples, o trace() vai mostrar o caminho percorrido pelo programa até chegar ao ponto em que a função console.trace() é chamada.

Vamos ver no código?
Para fazermos um teste, vamos criar um arquivo index.js e nele uma função chamada ola() e outra chamada mundo():


```
function ola(){
    function mundo() {
        console.trace('Ola Mundo');
      }
  mundo();
}

ola();
```


A saída no seu terminal será assim:

```
Trace: Ola Mundo
    at mundo (file:///<diretorio>/index.js:3:15)
    at ola (file:///<diretorio>/index.js:5:1)
    at file:///<diretorio>/index.js:8:1
    at ModuleJob.run (internal/modules/esm/module_job.js:140:23)
    at async Loader.import (internal/modules/esm/loader.js:165:24)
    at async Object.loadESM (internal/process/esm_loader.js:68:5)
```


Como podemos ver, o método console.trace() imprime a mensagem "Ola Mundo" no topo e depois apresenta todo o caminho percorrido nos locais em que o console.trace() foi chamado.

Aqui a função ola() é chamada primeiro e a função mundo() é chamada posteriormente (observe que na lateral direita aparece o número da linha em que o console.trace() é chamado, que é o número "3").

O console.trace() é muito vantajoso quando pensamos em cenários complexos, pois fornece um stack trace (rastreamento de pilha) completo, com informações sobre os locais, módulos ou arquivos em que os métodos são chamados.

Esse método funciona como ferramenta importante para encontrarmos bugs e atua de mãos dadas com o interpretador. Essa prática é possível graças ao motor de interpretação do JavaScript (também chamado de engine) que utiliza uma pilha de chamadas (call stack) como regra de execução de funções. A pilha de chamadas trabalha com a estrutura de dados conhecida como pilha, que tem como regra que "o último a entrar é o primeiro a sair" - uma sigla conhecida na programação como LIFO, last-in-first-out.

Isso significa que, sempre que executarmos um script, o motor JavaScript organiza a execução de forma global e insere a execução da última função chamada no topo de pilha de chamadas.

Imagine blocos empilhados um em cima do outro, ou uma pilha de pratos. Se tentarmos retirar o último bloco ou o último prato, o que acontece? Certamente tudo irá desmoronar, e é assim que a pilha de chamadas funciona também; o motor JavaScript executa a última função chamada e se uma função chamar outra em seu escopo, um novo contexto de execução será criado e colocará a nova função no topo da pilha de chamadas.

O script só finaliza a execução quando a pilha de chamadas estiver vazia.

Que tal pesquisar um pouco mais?

[console.trace()](https://developer.mozilla.org/en-US/docs/Web/API/console/trace_static)
[Call stack (Pilha de chamadas)](https://developer.mozilla.org/pt-BR/docs/Glossary/Call_stack)



### 9.8 QUICK SORT



#### Posicionando um Pivô


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/ab8e7c14-4439-47b9-ad90-8092ddfb84d5)

Segue mais ou menos a mesma linha do merge sort.

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/797ca312-3532-4f3b-9337-35c0323d7d92)



#### Ordenação pelo Pivô


Nesse momento já sabemos quantos elementos têm valor menor do que um dado elemento escolhido na nossa lista, que chamamos de pivô.

Esse código sozinho por enquanto não está fazendo muita coisa. Nós temos que usar a posição do pivô para posicionar o restante dos elementos de um lado ou do outro. Podemos dizer que ficam à esquerda do pivô os menores e à direita do pivô os maiores.

 Por enquanto só conseguimos posicionar o pivô no lugar dele trocando ele de lugar com outro elemento. No caso do exemplo usamos o Java como pivô, um elemento de 30, que podemos chamá-lo pelo seu valor, e localizamos cinco elementos com valor menor do que 30. A partir daí trocamos o Java de lugar com o elemento que estava na posição que ele deveria estar por enquanto.

E agora o que temos que fazer é a evolução, a próxima parte desse algoritmo, que é realmente empurrar todo mundo que tem valor menor para antes do pivô e quem tem valor maior para depois.

 Usamos o Java nessa simulação, e agora vamos fazer isso de uma forma um pouco diferente no algoritmo. Então vamos para o código.

 Eu vou começar criando mais uma função que eu vou chamar de function divideNoPivo().

O que recebemos nessa função por parâmetro? Um dos parâmetros é o array que essa função vai trabalhar; e poderíamos passar o pivô também, como tínhamos feito anteriormente passando o Java que era a posição 2 do array que estávamos trabalhando.

 Em termos de código, se formos pensar, o código vai ficar mais simples se pedirmos para pegar o primeiro elemento, por exemplo. Pegar sempre o primeiro elemento do array e usar como pivô, porque a posição do pivô vai andar, vai ser modificada.

 Mas não costuma ser uma boa ideia fazer isso, porque nós nunca sabemos qual é o array que vamos receber para trabalhar. E se o array já tiver internamente algum tipo de ordenação, pegar pelo primeiro vai resultar no algoritmo se comportando da pior maneira possível.

 O que podemos fazer é pegar o último elemento, pegar um elemento aleatório, considerando o começo e o fim do array, ou pegar sempre do meio.

 Já que nós já sabemos pegar o elemento do meio de um array, vamos manter o nosso código pegando sempre o elemento do centro.

 Então dentro da função “divideNoPivo” eu vou criar uma let que vou chamar de pivô mesmo, e ela vai receber o número do índice que corresponde ao meio do array, então let pivo = Math.floor(array.length / 2);. Passamos isso dentro de um método “Math.floor” para termos um valor arredondado para baixo.

 Agora já temos o pivô. Já vou pedir no final da função para retornar o array dividido com return array;.

 Então agora vamos pensar no que temos que fazer. Dava já para chamar função “encontraMenores”, que é a função que está trocando o pivô de lugar e o colocando no lugar certo dele.

 Então podemos chamar a função “encontraMenores”. E para funcionar ela precisa dos parâmetros pivô e array: encontraMenores(pivo, array);.

 Esses dois nós já temos, o array que será recebido como parâmetro da função mais externa, “divideNoPivo”; e a let pivo que acabamos de criar, que vai sempre pegar o elemento do meio e posicioná-lo no lugar dele, pensando que o elemento do meio não vai ficar no meio. Ele será usado como pivô e vai se movimentar de acordo com a quantidade de maiores e menores que o código vai descobrir que tem no array.

 Como funciona mesmo o “encontraMenores”? Ele vai contando a quantidade de elementos menores do que o pivô que tem no array. A partir disso ele sabe quantas posições tem que ter antes do elemento selecionado e posiciona.

 Então para conseguirmos passar os menores para o lado certo do array, que é a esquerda do pivô, podemos continuar usando a mesma lógica.

 Só que dessa vez vamos criar dentro da função “divideNoPivo” uma outra variável para ir controlando quantos menores nós encontramos.

Então vou criar uma let chamada “valoresMenores”, que vai começar com 0, que vai ser a primeira posição do array: let valoresMenores = 0;. Começamos com zero, e se já encontrou alguém menor, já coloca no 0.

E vamos aumentar, e se encontrar outro menor coloca no 1, coloca no 2 etc., é uma lógica bem parecida com a que utilizamos no “encontraMenores”. E agora vamos fazer um for para ir rodando esse array e vendo o que é maior e o que é menor.

Vou chamar a variável de controle do for de “analisando”: for(let analisando = 0;). Ela começa no índice 0 porque é o índice que estaremos analisando no momento.

 Enquanto “analisando” for menor do que o comprimento do array, vamos incrementar analisando no final de cada iteração: for(let analisando = 0; analisando < array.length; analisando++).

 Então já temos os índices que vamos trabalhar, lembrando que além dos índices precisamos puxar o dado, o objeto que vamos trocar de lugar ou não, analisar ou pegar o preço.

 Então dentro do for eu vou criar uma let atual, que vai ser o dado, o objeto que estaremos trabalhando no momento.

 E ele vai ser o resultado de array na posição “analisando”: let atual = array[analisando];. Lembrando que quando fazemos isso, o que está guardado dentro da let atual é o dado, o objeto com chave e valor.

E agora, dentro desse for nós colocamos nossa condição de comparação de preço, que é o valor que estamos usando para comparar.

 Então if(atual.preco < pivo.[preco]). Quando o valor atual que está sendo analisado é menor do que o pivô, ele tem que estar deslocado para a esquerda do pivô.

Lembrando que vai ter uma quantidade x de lugares, de elementos que vão estar antes. Então o nosso atual tem que ir para a posição que detectamos como menor. Lembra que começamos no zero.

 Então vamos chamar de novo a função “trocaLugar”, que precisa de array como primeiro parâmetro. O segundo parâmetro é onde o elemento que será trocado está no momento em que ele está na posição “analisando”, que é a posição do loop no momento.

 Então ele passa de analisando, que é o número do índice, e vai passar para “valoresMenores”, muito parecido com o que fizemos na função “encontraMenores”. Ele está no momento na posição analisando e ele passa para a posição “valoresMenores”: trocaLugar(array, analisando, valoresMenores).

 Lembrando que ambos os valores são números referentes ao índice do array que estamos trabalhando. Eu vou corrigir o meu pivo.preco que ficou escrito errado.

 E uma outra coisa que tem que acontecer dentro desse if é que se “valoresMenores” começa com 0 e colocamos um elemento, temos que atualizar o valor dessa variável, porque senão sempre que tiver um valor menor ela vai tentar entrar no índice 0.

 Então se já tem um elemento na primeira posição, no índice 0 do array, ele tem que depois ir para o índice 1. Então vamos aumentar: valoresMenores++.

 E o próximo elemento que tiver o valor menor do que pivô, ele vai executar o troca de lugar passando “valoresMenores”. Só que o “valoresMenores” terá o valor de 1. E ele vai entrar como segundo elemento do array, no índice de número 1.

 Então só tem uma coisa que precisamos fazer: no nosso if tem uma verificação a ser feita. Nós vamos passando pelo array, mas não podemos fazer o pivô comparar com ele mesmo.

 Então dentro do if vamos colocar “&&”, com a condição “e”, dizendo que o atual tem que ser diferente do pivô, então if(atual.preco < pivo.preco && atual !== pivo). O atual não pode ser o pivô, porque senão vai tentar mudar o pivô que já estava no lugar certo, e não queremos isso.

Vamos testar no final do arquivo: console.log(divideNoPivo(listaLivros));. Vamos no terminal então. Já estou na pasta certa, vou executar node encontraMenores.js.

 Tem um erro no meu código, vamos dar uma olhada. Tem um erro que eu já percebi: a nossa condição não precisa ser exatamente menor, ele pode ser menor ou igual, então fica if(atual.preco <= pivo.preco && atual !== pivo).

 Essa foi a primeira coisa que eu vi, mas não é disso que ele está reclamando. Ele está reclamando que a propriedade preço não existe no tipo number.

 Na linha 26, na primeira linha dessa função, eu passei a variável pivô, e ela está guardando um número. Só que ela deveria guardar um valor, não um número, deveria guardar um dado.

 Inclusive porque no if da linha 32 eu chamo pivo.preco, e obviamente, se a minha variável pivô é o resultado de array.length / 2, vai ser um número.

 Então isso não deveria ser um número. A let pivô deveria ser array na posição Math.floor(array.length / 2). Então corrigindo fica let pivo = array[Math.floor(array.length / 2)];.

 Aí sim vai pegar o valor do array, dividir por 2, arredondar para baixo, isso vai virar um número, um índice, que é a posição desse índice no array. Então o que terá salvo em pivô é um dado. Podemos inclusive fazer um console.log(pivo) para ver se está tudo certo.

Agora já deve ter corrigido. Vamos tentar rodar mais uma vez. Então node encontraMenores.js. O pivô é um dado, vamos ver se deu tudo certo.

 Voltando no array original, o objeto que tinha o livro Rust é o meio do array. Vamos ver a situação que está agora. No array ordenado ele passou para o terceiro elemento, o elemento no índice 2. Nosso array está ordenado, e antes dele tem apenas dois outros livros, de valores 15 e 20.

 Realmente, se formos olhar todos os valores do array, são os únicos dois livros que têm valores menores que 22. No caso tem que ser menor ou igual, mas não tinha nenhum igual.

 Então agora sim o nosso array está ordenado, nosso código está funcionando. Nosso código “divideNoPivo” consegue separar os menores dos maiores.

 Nós ainda não cuidamos da organização interna, da ordenação entre as partes menores e maiores, mas calma que vamos chegar lá.


Resultado:
![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/3593f5c1-06ad-4b11-b8d5-3fd12885994c)



#### Quick Sort


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/e406d8b1-66d6-4649-a942-f66118b452df)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/dce63957-627e-48be-873d-53d215773f36)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/b23e6a28-f5a7-489c-87ce-b63997b48a62)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/d3ffda9f-1666-46e6-9c8e-cb4fb6d38cec)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/45fb2c97-58bf-479a-ab39-ac657950e833)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/1cd32ac2-d5f4-4526-b996-48a7828f8e30)


Vejamos então como aproveitar toda essa lógica que construímos até agora para não só a partir de um pivô separar valores menores e valores maiores, mais sim terminar ordenando o array completamente.

 Vão existir ocasiões em que pode ser útil você apenas separar menores para um lado e maiores para o outro, mas vamos considerar o caso de uma ordenação completa.

 O pivô do array que trabalhamos no código anterior começa no elemento de valor 22, que é o Rust. É o meio da lista.

 Se considerarmos esse pivô e ordenarmos como já fizemos, nós descobrimos que só existem dois elementos com valor menor do que o de Rust na lista.

 E a partir do momento em que identificamos que só tem dois elementos menores, conseguimos posicionar o Rust no lugar dele, o terceiro elemento do array, que é o índice 2, trocando ele de lugar com o elemento que estava anteriormente, que é o Java de 30. Então os dois elementos trocaram de lugar e agora o pivô está posicionado no lugar dele com relação ao array completo.

 Como conseguimos expandir isso? Pensando da mesma forma que fizemos anteriormente, em que tanto a lista que está para a esquerda quanto a lista que está para a direita são duas listas separadas. E conseguimos aproveitar a lógica para cada uma delas, sempre começando do lado esquerdo.

 Então vamos terminar o que tem para o lado dos menores que o pivô. Nesse pequeno array de dois elementos, que são os menores, vamos estabelecer um novo pivô, que é o Python, o segundo elemento do array, o elemento de número 1.

 Então a partir dele como pivô conseguimos organizar esse array, fazendo da mesma forma que fizemos anteriormente, jogando para a esquerda os maiores e para a direita os menores.

 Só que agora só temos dois elementos, um de cada lado. Nesse caso, em que estamos trabalhando com um array de poucos elementos, é mais fácil de cair nas coincidências. Por coincidência a ordenação já colocou 15 e 20, os dois em ordem. Mas como eu disse, é uma coincidência, mesmo assim o código vai passar para fazer essa verificação.

 Então temos um novo pivô, a partir desse pivô um array de dois elementos, um está para um lado e um para o outro. Conseguimos ordenar esses dois. E agora todo o lado esquerdo, o lado de menores do que o nosso pivô original, que foi Rust, já está ordenado.

 O que sobra são todos os elementos do lado direito, os elementos maiores do que o pivô original. E agora temos o que podemos considerar como um array somente desses elementos. Vamos ver como fica então.

 Criando a partir só dos elementos do lado direito, rodamos a lógica novamente, e temos um novo pivô, no caso, o Ruby de 28.

 Vamos fazer mais uma verificação, olhar nessa lista de todos os que sobraram quantos elementos tem de valor menor do que 28.

 Só tem um, que é o JavaScript. Nós sabemos que nesse array menor temos um espaço de um elemento e o Ruby é o segundo elemento, que seria do índice 1. Nós trocamos de lugar. Então o que estava antes nesse lugar era o Elixir, trocou de lugar com o Ruby.

 E a partir disso é a mesma lógica: os menores vão para a esquerda e os maiores para a direita. Agora só temos um elemento menor, que é o JavaScript, que ficou no lugar dele.

 E o que nós temos agora é mais uma lista pequena, com menos elementos, mas que também vamos repetir o mesmo processo.

 Agora a partir do pivô dessa lista menor, temos só o JavaScript para o lado esquerdo. Ele está sozinho, não tem com quem “pivotar”, então ele já está ordenado.

 E agora novamente, verificamos quantos elementos existem nesse pequeno trecho de array dos que são menores do que 45. Temos um de 30, um de 40, um de 33 e um de 35.

 Então sabemos que Go se posiciona como o quinto elemento depois dos 4 menores. Ele vai para o lugar, trocando de lugar com o elemento anterior.

No caso, temos para a direita de Go dois elementos menores do que ele. Então na hora que essa troca é feita, o código primeiro vai trocar o Go de lugar com o C#, e depois, na hora que for passar o Elixir como o único elemento maior, ele vai também trocar de lugar com C# e depois trocar de lugar com o C++ e fica tudo no lugar.

Continuando, agora nós temos do lado direito do Go um elemento só, que não tem com quem “pivotar”, ele já está ordenado. E para o lado esquerdo temos quatro elementos, e vamos repetir o processo.

 Agora o pivô é o C#. Colocando o C# no lugar, nós temos só um elemento de valor menor do que o C#. O C# custa 33, e só tem o Java de 30.

Então sabemos que tem espaço de um elemento e o C# tem que ser o segundo. Posicionamos o C#, trocando ele de lugar com o que estava anteriormente, que é o Scala.

 Quando a lógica é processada, o Java, que é o único elemento de valor menor do que 33, vai para o lugar dele na esquerda, e agora é um só. E do lado direito nós temos apenas dois elementos que sobraram.

 E agora, a partir desse momento só temos um elemento do lado esquerdo, que já está ordenado e não tem com quem “pivotar”.

 E do lado direito o pivô agora é o C++, ele é menor do que Scala. Agora temos um elemento de cada lado, eles podem trocar de lugar e automaticamente dessa forma ordenar só essa parte que falta.

 E o resultado final é um array completamente ordenado, onde começamos a partir de um pivô, fazemos tudo para a esquerda, depois fazemos tudo para direita.
 E qual é a intenção dessa lógica? É ir reduzindo aos poucos o tamanho de cada pequeno array até que tenha apenas dois elementos. Quando você tem só dois elementos você troca os elementos de lugar se for necessário.

 Então essa é a base de um algoritmo de ordenação que chamamos de quick sort, de ordenação rápida, que é particionar a partir de um pivô, ordenar à esquerda, ordenar à direita até que o array esteja reduzido a um elemento. Com um elemento de cada lado você consegue ordenar e trocá-los de lugar se necessário.

 Agora podemos começar em pequenos passos a pensar em como implementar isso em código.



#### Entendendo o código


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/52004800-1896-4fa3-9346-bbf7c8cf677c)


Vamos então fazer a implementação desse algoritmo que conversamos no JavaScript. Na pasta da aula eu vou criar um novo arquivo chamado “quickSort.js”. E já na primeira linha não podemos esquecer de importar a nossa lista de livros: const listaLivros = require(‘./array’);.

A primeira coisa que eu vou fazer é criar a função do quick sort. Vamos lembrar um pouco do merge sort que trabalhamos anteriormente.

 A primeira coisa que eu vou fazer é criar uma função parecida com merge sort, só que agora vamos trabalhar com outro algoritmo. Mas o princípio será muito parecido: é uma função que, como temos que pegar um array e ir dividindo e diminuindo, vamos trabalhar com o mesmo princípio de recursão.

 Então vou criar primeiro uma função que eu vou chamar de quick sort: function quickSort(). Essa função precisa receber o array que ela vai trabalhar, e também, lembrando que estamos trabalhando com um array só, precisa passar a posição onde ela começa a trabalhar e onde ela termina de trabalhar, ou seja, o índice de início e o de final.

 No quick sort trabalhamos muito com o conceito de parte da esquerda e da direita do pivô. Então vamos passar como segundo e terceiro parâmetro “esquerda” e “direita”, que é a parte esquerda, o índice de início, e a parte direita, onde seria o índice de final onde o array precisa encontrar o pivô e fazer a ordenação. Então function quickSort(array, esquerda, direita).

 Na última linha da função já vou pedir para retornar o array que será o array organizado, ordenado: return array;. E na última linha do arquivo já deixo o quick sort chamado com “listaLivros”, então faço console.log(quickSort(listaLivros)).

 E como na última linha do arquivo é onde será feita a primeira chamada da função, já passamos o índice de início, que é o 0, a primeira posição do array e o final, que é listaLivros.length.

 Porém, passamos listaLivros.length - 1 porque length é uma propriedade que traz a quantidade de elementos. E não queremos a quantidade de elementos, queremos o índice do array. Lembrando que o array começa com 0, então é length -1.

 Como já tínhamos visto anteriormente, temos que diminuir o array até que ele seja um array de um elemento, para então você fazer a comparação entre dois.

 Então vamos dizer que só vai executar o que está dentro da função quick sort se o array.length que for passado como parâmetro for maior do que 1: if (array.length > 1).

 Se for menor, já vai retornar só o que tem no array, o elemento dele. Então dentro desse if é que vamos desenvolver toda a parte de recursão, de ficar chamando a função.

 E dentro, da mesma forma que fizemos com o merge sort, vamos fazer as chamadas recursivas e fazer a parte de ordenação. Então a primeira coisa que temos que pegar no nosso quick sort é criar uma let que eu vou chamar de var temporária, porque ainda não sabemos o que virá.

 E dentro dessa var temporária eu vou criar uma função parecida com a função “ordena” que é chamada no merge sort, só que eu vou chamar essa função de “particiona”, que é o que ela está fazendo na verdade: let varTemp = particiona().

Essa função “particiona” também vai receber o array que ela vai trabalhar, a parte esquerda, onde tem que começar, e a parte direita onde tem que parar: let varTemp = particiona(array, esquerda, direita).

 Lembrando que cada vez que essa função for chamada ela vai receber novos valores de início e de fim do array.

 Agora vamos escrever a nossa função particiona. Então function particiona(). Ela vai receber o array, a parte esquerda e a parte direta do array, que é o índice onde ele para de percorrer: function particiona(array, esquerda, direita).

 A primeira coisa que tem que fazer na hora que pegamos um array para fazer o quick sort é achar o pivô. E o pivô pode ser encontrado de várias maneiras, colocado no começo do array, colocado no final, um número aleatório, mas vamos manter no meio.

 Então vou criar uma let pivô, lembrando que queremos pegar o dado, porque o objeto é onde tem o valor, o título e o valor do livro, que é o que queremos comparar.

 Então tem que ser array na posição Math.floor para trazer um número arredondado. E vai ser o resultado de (esquerda + direita) / 2, colocando “esquerda + direita” entre parênteses para que essa operação seja feita primeiro: let pivo = array[Math.floor((esquerda + direita) / 2)].

 Ou seja, vamos somar o índice passado como esquerda e passado como direita e dividir por 2. E assim conseguimos ter o número, o valor do pivô. Ou seja, quando fizermos a primeira chamada da função, vai começar no zero, que é o primeiro índice, vai terminar no 10, porque estamos trabalhando com uma lista de 11 elementos.

0 + 10 dá 10, dividindo por 2 dá 5. Então vai estar no índice 5, o sexto elemento. E sucessivamente, a partir do momento que formos diminuindo o array, vai ser a mesma lógica.

 E agora vamos pensar um pouco melhor em como vai funcionar esse particiona. Para fazer um for que percorre todos os elementos, vê quantos tem menor, encontra a posição do pivô e só depois movimenta o pivô é muita coisa. Vamos tentar fazer isso de uma forma um pouco diferente e mais performática.

 Vamos pensar dessa forma: temos uma lista de 10 elementos que começa no zero e vai até o 10, que é onde queremos começar. Fazendo isso, encontramos o pivô no elemento de valor 22, que é o sexto elemento, ou elemento de índice 5.

 Nós sabemos que tudo que tem valor menor do que 22 tem que estar à esquerda do pivô, e tudo que tem valor maior tem que estar à direita. Então começamos verificando quais elementos do lado esquerdo não deveriam estar lá, ou seja, os elementos de valor maior.

 Nós começamos a fazer isso a partir do índice 0, a partir de onde começa o nosso trecho de array.

Então logo o primeiro elemento já tem valor maior, porque 45 é um valor maior do que o pivô, que é 22. Então já temos um elemento que está no lugar errado. Vamos parar por aqui, vamos segurar o índice desse elemento, que é o índice 0.

 Vamos então passar para o outro lado e ver se eu tenho algum elemento do lado direito que não deveria estar lá, porque assim eu posso trocar os dois de lugar.

 Já o último elemento do array, o elemento de índice 10, já é menor do que o pivô, então ele também está no lugar errado. O que fazemos então? Trocamos esses dois elementos de lugar.

 Trocamos o de 20 e o de 45. Vamos continuar percorrendo para a esquerda, lembrando que sempre começamos na esquerda.

 O próximo elemento do índice 1, o 35, já é maior do que 22, então 35 também está no lugar errado. Segura esse elemento, esse índice. Vamos ver se podemos trocá-lo de lugar com alguém que está do lado direito.

 Do lado direito temos 33, que não é menor do que 22, então está no lugar certo. 25 não é menor do que 22, também está no lugar certo. Temos 28, depois 40 e chegamos no pivô.

O pivô não tem valor menor do que o pivô, podemos considerar que tem valor igual. Mas ele ainda está no lugar errado com relação ao 35, que é onde paramos na esquerda. Então trocamos eles de lugar também.

Vamos trocar o pivô de lugar. Lembrando que o pivô se movimenta também. Ele começa no centro, mas não quer dizer que vai ficar no centro. Mas nessa iteração ele continua sendo o pivô.

 O atual da esquerda é o 30. 30 é maior do que 22. Apesar de eles terem trocado de lugar, 30 ainda é maior do que 22. Então vamos segurar esse elemento. A comparação ainda está sendo feita com o pivô, então segura o 30.

 35 é maior, então está certo, a parte da direita está certa ainda. 50 é maior do que 22, está certo ainda. Lembrando que estamos diminuindo, decrementando o índice.

 Chegamos no 15. 15 é menor do que 22. Então podemos fazer a mesma coisa que fizemos anteriormente. Vamos trocar o índice atual que está guardado na esquerda com o índice atual da direita. Então trocamos Java com PHP.

 Continuamos andando, só que se continuarmos decrementando a direita e incrementando a esquerda, eles se cruzam. A partir do momento que ele se cruzam, se continuamos com essa mesma lógica, essas variáveis vão ficar andando de um lado para o outro.

 Então a partir do momento que ele se cruzam, que o valor do índice da esquerda não é mais menor do que o índice da direita é a hora que temos que parar essa iteração e ver o que aconteceu.

 Para a esquerda do meu índice atual eu tenho já três elementos que são menores, 20, 22 e 15. E esses elementos não estão ordenados entre si. Então nesse momento nós paramos e passamos o valor atual da minha variável que está controlando os índices da esquerda como referência para a próxima iteração, para a próxima chamada da função.

 Então a próxima chamada da função vai ser do 0 até um índice antes do que paramos. Então ele vai percorrer o índice 0, o índice 1 e o índice 2.

 No final desse processo teremos nosso pequeno array de três elementos, 20, 22 e 15, alinhados entre si. E é fazendo essas pequenas partes de alinhamento que esse algoritmo vai funcionar.


#### IMplementando o codigo


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/1910f0ad-97db-4788-85e8-ad800e71404d)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/396eac35-3f30-43dd-b6d6-de0ce34140ee)

Então se o índice da atual esquerda for menor ou igual ao índice da atual direita, nós trocamos de lugar: if (atualEsquerda <= atualDireita). E já temos um algoritmo pronto para trocar de lugar, que está dentro do meu arquivo “trocaMenores”, é a função “trocaLugar”.

 O que podemos fazer então no final do arquivo “encontraMenores.js” é um module.exports = trocaLugar;.

 E importamos dentro de “quickSort.js” a função “trocaLugar” para podermos usá-la. Então no começo do arquivo fazemos const trocaLugar = require(‘./encontraMenores’);. E vamos usar essa função dentro do nosso if. Se for menor nós chamamos a função “trocaLugar”.

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/3e72f087-8b9f-4d91-9b4d-3fea7fa3aa76)

![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/96b77cfc-55b6-4624-be48-a81b9f64c72d)

testa no terminal, e ele deve retornar um array ordenado.

Uma implementação “oficial”?

Durante o curso, temos abordado cada algoritmo a partir do conceito, passando pela representação em diagrama/teste de mesa, para só depois implementar o código. O que pode gerar a pergunta: Existe mais de uma forma de implementar um algoritmo?

A resposta é: sim. O código, com suas funções e métodos utilizados, pode variar e depende inclusive da linguagem utilizada. É possível encontrar o mesmo algoritmo implementado de formas diferentes. Porém, a lógica de funcionamento do algoritmo sempre permanece a mesma. Por esse motivo não começamos direto pelo código e sim entendendo como o algoritmo é pensado e como ele deve se comportar.

Durante o curso, desenvolvemos primeiramente um código mais “agnóstico”, para em seguida utilizar mais métodos como, por exemplo, array.push(). Mas seria possível desacoplar ainda mais, abstraindo funções de comparação para não depender de uma propriedade objeto.preco, por exemplo.

Você pode testar suas próprias ideias ou pesquisar outras implementações. 



####  Revisando valoresMenores


Durante a aula, utilizamos a variável valoresMenores na função divideNoPivo(). Vamos analisar esta variável para entender como ocorre a troca de posições no array.

A primeira coisa que a função divideNoPivo() faz é localizar o pivô no meio do array (no array que usamos na aula é a posição listaLivros[5], ou seja: { titulo: “Rust”, preco: 22 }. Em seguida, chama a função encontraMenores() que vai contar quantos elementos com valor menor que 22 existem no array, para em seguida trocar o pivô de lugar com o elemento que está na posição seguinte à quantidade de elementos menores.


```
function divideNoPivo(array) {
 let pivo = array[Math.floor(array.length / 2)];
 encontraMenores(pivo, array);

 return array;
}
```


Em seguida, é feito um loop para passar os elementos com valor menor que o pivô para a esquerda dele, e os de valor maior para a direita.

A variável atual guarda o objeto referente ao elemento que será comparado com o valor do pivô, e é dessa variável que pegaremos a propriedade preco.


```
function divideNoPivo(array) {
 let pivo = array[Math.floor(array.length / 2)];
 encontraMenores(pivo, array);
 let valoresMenores = 0;

 for(let analisando = 0; analisando < array.length; analisando++) {
   let atual = array[analisando];
 }

 return array;
}
```

Chegamos à condicional `if`, que faz a comparação do preco entre o pivô e o atual. Caso o preço do elemento atual seja menor, chamamos a função trocaLugar para trocar a posição do elemento atual com o elemento na posição valoresMenores - lembrando que o valor inicial dessa variável é `0`, o que corresponde ao índice do primeiro elemento do array.

Em seguida, o valor da variável `valoresMenores` é incrementado.


```
function divideNoPivo(array) {
 let pivo = array[Math.floor(array.length / 2)];
 encontraMenores(pivo, array);
 let valoresMenores = 0;

 for(let analisando = 0; analisando < array.length; analisando++) {
   let atual = array[analisando];
   if(atual.preco <= pivo.preco && atual !== pivo) {
     trocaLugar(array, analisando, valoresMenores)
     valoresMenores++
   }
 }

 return array;
}
```


Destrinchando o intuito da variável valoresMenores: ela está controlando a posição onde serão inseridos os elementos com valores menores que o pivô - lembrando que nesse momento o pivô já está posicionado em seu índice correto.

Por esse motivo valoresMenores é iniciada no índice 0: durante o laço for, cada elemento do array tem sua propriedade preco comparada com preco do elemento pivô. Quando é encontrado o primeiro elemento com valor menor (PHP no índice 3), o código entra no bloco if e chama a função trocaLugar() passando como parâmetros de troca a posição do elemento atual e a posição 0, que é o valor da variável valoresMenores neste momento da execução.

Isso vai fazer com que um elemento de valor menor que o pivô assuma o lugar de um elemento de valor maior.

Ou seja, após a primeira execução da função saímos de:

```
[
 {
   titulo: "Go",
   preco: 45
 },
 {
   titulo: "C++",
   preco: 35
 },
 {
   titulo: "Java",
   preco: 30
 },
 {
 titulo: "PHP",
 preco: 15
 },
 {
   titulo: "Elixir",
   preco: 50
 },
 {
   titulo: "Rust",
   preco: 22
 },
 // restante dos elementos
]COPIAR CÓDIGO
Após o posicionamento do pivô:

[
 {
   titulo: "Go",
   preco: 45
 },
 {
   titulo: "C++",
   preco: 35
 },
 {
   titulo: "Rust",
   preco: 22
 },
 {
 titulo: "PHP",
 preco: 15
 },
 {
   titulo: "Elixir",
   preco: 50
 },
 {
   titulo: "Java",
   preco: 30
 },

 // restante dos elementos
]
```


E quando o for chega no quarto elemento (índice 3), localiza pela primeira vez um elemento do array com valor menor que o pivô. Então o valor de valoresMenores é `0` e o elemento PHP de valor 15 trocará de lugar com Go de 45.

```
[
 {
   titulo: "PHP",
   preco: 15
 },
 {
   titulo: "C++",
   preco: 35
 },
 {
   titulo: "Rust",
   preco: 22
 },
 {
   titulo: "Go",
   preco: 45
 },
 {
   titulo: "Elixir",
   preco: 50
 },
 {
   titulo: "Java",
   preco: 30
 },

 // restante dos elementos
]
```


Após a troca, valoresMenores é incrementada em `1` (com a linha valoresMenores++). Dessa forma, da próxima vez que o for localizar um elemento com valor menor que o pivô, ele será trocado pelo elemento que está no índice `valoresMenores` ou seja, `1`.


### 9.9 BUSCA BINARIA


####  Dividir para Buscar


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/80ef0ea4-43d6-4832-9acc-09ec2e49dbbe)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/9069e541-c3d6-47ba-bc54-8c572ebe5a5e)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/7f55cd9a-c669-4933-8d3b-5f2eba972171)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/08c55f69-1dce-4df4-abc8-f8f9b4f2c6ce)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/16dbcd13-7602-46cb-8f34-62e93478a77e)



 como seria se, ao invés de um algoritmo de ordenação, tentássemos utilizar isso em uma busca?

Por exemplo, até agora nos algoritmos de busca que vimos, aquele primeiro que pensamos em implementar com for vai percorrer todo um array para encontrar e devolver o elemento, ou ir até o final para dizer que não encontrou o elemento.

 Se tentássemos dividir a busca em partes, será que funcionaria melhor? Vamos ver então com um exemplo mais do mundo real.

 É possível que você já tenha feito a seguinte brincadeira: eu vou pensar num número de 1 a 10 ou de 1 a 100, tanto faz, e você vai tentar adivinhar qual é esse número com a menor quantidade de chutes necessária.

 Então se meu número é 50 e você chuta 25, eu falo “mais”, se for um número maior, ou “menos”, se for um número menor.

 Como seria a melhor estratégia para um jogo como esse? Normalmente a pessoa vai ajudar quem está tentando chutar dizendo “menos” ou “mais”. E se simulássemos esse jogo com um número de 1 a 10 para ficar mais fácil de visualizar, ao invés de 1 a 100?

 Vamos tentar simular e pensar assim: a pessoa pensou no número 7, e eu vou começar a chutar. Eu chuto o número 5, por exemplo. E a pessoa vai falar “mais”, porque eu chuto no 5 e o número é 7.

 Nesse momento nós descartamos automaticamente tudo que é de 5 para baixo, porque ela falou que é mais, então não tem porque eu ficar chutando 3, por exemplo, que não tem nada a ver.

 E se é uma lista de 10 números e eu chuto bem no meio e erro, eu já consigo descartar metade de uma lista, ou para cima ou para baixo, depende se a pessoa fala “mais” ou “menos”.

 E como seria o próximo chute? Nós podemos seguir sequencialmente, chutando 6, 7 e assim por diante, mas não é a melhor alternativa. Nós poderíamos aplicar essa mesma lógica para chutar 8, que é mais ou menos no meio, e tentar descartar novamente metade da lista.

 Eu chuto 8, a pessoa vai falar “menos”. Só que com essa abordagem, com dois chutes eu já descartei quase todos os números. Sobrou apenas 6 e 7.

 Ou seja, eu consigo acertar um número em no máximo três chutes. Descartei a metade, depois descartei metade da metade, e apenas com 3 chutes no máximo eu consigo acertar, porque eu vou direto no número certo ou eu vou descartar o número que está errado e ter o número certo por redução de possibilidades.

 Se aplicássemos isso, por exemplo, para uma lista telefônica ou uma lista de produtos ordenados por preço, nós meio que já utilizamos essa lógica sem perceber na cabeça.

 Então se eu estou procurando numa lista um produto de R$ 30, eu dou uma olhada no começo da lista e o primeiro preço é 15, olho o último preço e é 50, nós meio que já sabemos mais ou menos onde procurar. Nós não vamos passar por 15, 20, 21, 22, 23, nem o contrário. Nós encurtamos, fazendo isso mentalmente. Eu vou direto na margem mais ou menos onde está o 30.

 É a mesma coisa numa lista ordenada em ordem alfabética. Se seu nome começa com J você não começa procurando o seu nome na lista no A. Você não precisa, você pode ir direto no começo do J e encontrar.

 Se é “Ju” de Juliana, então não está no “Ja”, de Janaína, eu posso tentar achar o final dos que começam com J, porque é mais provável que o meu nome esteja lá.

 E nós já fazemos isso normalmente na nossa cabeça. E da mesma forma que fizemos com o jogo de acertar o número, nós conseguimos reduzir uma lista. Por exemplo, se eu quero mais ou menos no meio, tiro os muito baratos e os muito caros, e conseguimos acertar com uma quantidade bem menor de chutes.

 Ou seja, no código nós conseguiríamos acertar o elemento que estamos buscando com uma quantidade bem menor de operações do que ficar procurando A, B, C, D, E quando eu quero o J, ou no 1, 2, 3, 4, 5 quando eu quero o 20, por exemplo.

 Se considerarmos um array de mil elementos, a lógica vai ser parecida: dividimos de mil para 500, de 500 para 250, de 250 para 175 e por aí vai.

 Vamos sempre diminuindo a lista, ou seja, numa quantidade muito menor de operações fica bem menor, mas mesmo assim o crescimento em quantidade maior de operações também não vai ser tanto assim.

 Vamos tentar implementar um algoritmo que traduza essa divisão para conquista para fazer uma busca.


####  Busca Binária


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/3500b1f3-7b1f-4fe6-baed-ce8294b805d2)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/28e9a38b-1ad9-41a8-b16d-ce026761fb57)

Testa no terminal.

Vamos tentar rodar com um valor que nao existe na lista:


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/91d7e94e-86ce-48b2-a93a-ba46a2fce13c)


Vamos fazer essa implementação em código do que nós vimos anteriormente. Eu já vou deixar pronto também um arquivo chamado “arrayOrdenado.js” com a lista de livros que já estamos trabalhando, porém agora já ordenada, pronta para fazer a busca. Dentro da pasta eu vou criar um arquivo que eu vou chamar de “busca.js”.

 A primeira coisa a fazer, como sempre, é importar a nossa lista livros: const listaLivros = require(‘./arrayOrdenado’);. E vamos criar a nossa função: function busca(). E o que essa função precisa receber? A primeira coisa será o array que vamos trabalhar: function busca(array, ).

E lembrando do que fizemos anteriormente no merge sort e no quick sort, a cada vez que executarmos a função busca, ela terá que fatiar o array e trabalhar com partes cada vez menores. Então começa com o array inteiro, e se o valor buscado for menor vamos cancelar toda a parte direita do array.

 Então a cada chamada de função nós precisamos passar para ela o que eu vou chamar de “de” e “até”, ou seja, o índice onde começa a fazer a busca e o índice até onde vai, porque estaremos trabalhando com fatias do array.

 Então o segundo parâmetro eu vou chamar de “de” e o terceiro de “até”: function busca(array, de, ate).

E o quarto parâmetro será o valor buscado, porque obviamente precisamos passar alguma coisa para essa função buscar para nós e eu vou pedir para retornar o índice onde está o elemento; ou não, se não encontrar nada. Então fica function busca(array, de, ate, valorBuscado).

 Revisando então como o algoritmo tem que funcionar: a cada vez que chamamos a função, tem que pegar um elemento sempre do meio do array e verificar. Por exemplo, se o elemento buscado é de 22 e o do meio é de 30, significa que o elemento buscado tem um valor menor, então ele estará à esquerda do elemento do meio. Lembrando que estamos trabalhando com um array já ordenado.

 E o contrário, se por exemplo, o valor buscado é 40 e valor do meio é 30, significa que o valor buscado está em algum lugar à direita, então temos que procurar à direita do meio e podemos descartar todo o resto.

 Então o que temos que fazer primeiro é encontrar o meio. Então vou criar uma const meio. Agora não é mais pivô, porque sempre estaremos trabalhando com o meio do array, e esse meio do array não vai se movimentar durante o processamento da função a cada iteração. O meio é sempre o meio.

 E será o resultado de Math.floor, e passamos “(de + até)”, a mesma coisa que fizemos anteriormente. Passamos o índice de começo e o de final e dividimos por dois. Eu vou englobar “de + até” com parênteses para fazer essa operação primeiro, então const meio = Math.floor((de + ate) / 2);. E com isso já temos o meio.

 Eu vou criar outra const que eu vou chamar de atual, que será o array na posição meio, porque temos o objeto e conseguimos acessar a propriedade preço para fazer a comparação: const atual = array[meio];.

 A partir disso temos três coisas possíveis que podem acontecer. A primeira coisa que pode acontecer é o elemento do meio ser exatamente o elemento que estamos buscando. Então pode acontecer da primeira vez ou podemos percorrer esse array até que isso aconteça.

 Então se o valor buscado for igual ao preço atual, nós só retornamos o meio, porque já é o índice onde está o valor que estamos buscando: if (valorBuscado === atual.preco) { return meio; }. Acabou processamento por aqui e saiu da função.

 Temos outros dois casos possíveis. Um deles é se o valor buscado for menor do que o preço atual. Isso significa que temos que procurar em alguma parte do array: if (valorBuscado < atual.preco).

 E o outro caso é se o valor buscado for maior do que o preço atual, e então temos que buscar em outra parte do array: if (valorBuscado > atual.preco).

 E agora nós vamos usar a recursão para fazer a busca se chamar da mesma forma que fizemos com o merge sort e o quick sort. Porque cada vez que chamarmos a função busca, vamos passar valores atualizados de início e de fim do array para fazer a busca dentro dele.

 E vamos fatiar esse array até que caia na situação de valor buscado ser igual ao preço atual, e nesse caso em que encontrou o elemento, retorna o índice do elemento e fecha o processamento.

 Então dentro do primeiro if, em que o valor buscado é menor do que o preço atual, nós temos que retornar busca, passando agora como parâmetro array: return busca(array, ).

 E vamos ver quais são os valores de “de” e de “até” que temos que passar. Se o valor buscado for menor do que o preço atual, isso significa que podemos descartar tudo que está à direita do valor do meio, inclusive ele.

 Então nesse caso quais seriam os valores atualizados de “de” e de “até”? O de “de” continua sendo o primeiro índice que passamos, o índice 0, no caso da primeira chamada da função.

 Nós continuamos trabalhando com o mesmo “de”, no caso, o índice 0 que depois vai mudar. Só que agora até onde vai nossa busca? Nossa busca não precisa mais ir até o final, ela pode parar antes do meio, porque o meio para o final já foi descartado.

 Então a nossa busca vai começar onde já estava começando, no caso, no índice 0, e depois vai continuando, e vai parar antes do meio.

 Ou seja, a condição de início continua sendo “de”, só que agora a condição de parada vai ser meio menos um: return busca(array, de, meio -1).

 Então vamos começar onde já estava começando, só que agora paramos antes do meio, descartando toda a parte do meio para a direita. E o valor buscado continua sendo o mesmo, e retorna esse valor: return busca(array, de, meio -1, valorBuscado);.

 A outra condição, que é valor buscado maior do que o preço atual, vai ser a mesma lógica, só que vamos buscar numa parte diferente do array. Começamos passando o array como parâmetro: return busca(array, ).

 O “de” agora não é mais o começo. Se o valor buscado for maior do que o meio, fazemos o contrário: descartamos do começo até o meio. Então nosso valor de início passa a ser 1 depois do meio, porque nós descartamos o meio e tudo que vem antes dele. Então o valor de início agora, ao invés de “de”, é “meio + 1”: return busca(array, meio + 1).

 E o índice de parada, até o final do array, é “até”, que já era onde estávamos parando: return busca(array, meio + 1, ate). E o valor buscado continua sendo o mesmo: return busca(array, meio + 1, ate, valorBuscado).

 Agora vamos testar a função, passando console.log(busca(listaLivros)). A condição de início da primeira chamada da função é o índice 0, o final vai ser listaLivros.length -1, como já fizemos nas outras vezes: console.log(busca(listaLivros, 0, listaLivros.length -1)).

 E o valor buscado vamos fazer um teste com o 40. Vou passar o 40, que é o índice 8 do nosso array. Então vou passar 40, que é o valor buscado: console.log(busca(listaLivros, 0, listaLivros.length -1, 40)).

 E vamos para o terminal. Eu já estou na pasta certa, vou chamar node busca.js. E ele retornou o índice 8, ou seja, está funcionando. Mas o que acontece se de repente passarmos um valor que não existe?

 Eu vou tentar antes passar novamente essa função com um valor menor para ver se funciona. Então vou tentar, por exemplo, o 20, que é o índice 1. Então vou chamar a mesma função passando 20 como parâmetro: console.log(busca(listaLivros, 0, listaLivros.length -1, 20)).

 Rodamos novamente no terminal e ele retorna o índice 1. Está funcionando. Só que o que acontece se eu passar, por exemplo, 60, que é um valor que não tem? Vamos tentar rodar novamente com 60.

 Ele deu um stack overflow, aconteceu um erro. Quando o node entra num loop infinito ele vê que já não dá mais para colocar processamento nessa pilha, então ele para de executar. Vamos ver o que aconteceu no próximo vídeo.



#### Refatorando a Busca


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/bf41ffc2-98f5-46f8-b31d-e22808193e32)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/9e21c95c-9dc5-4af4-8c3e-ede8b905fa62)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/c8d46393-0939-45be-9607-028fba4783e4)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/15518941-1fdf-4001-8b38-e19793fe0ee9)


Implementamos o algoritmo da nossa busca, porém, o que acontece quando passamos um elemento que não existe na lista? Ele deu erro. E pode acontecer quando fazemos uma busca de o elemento não existir. E não pode dar erro nesses casos.

 O que tivemos nessa situação foi um erro de pilha. Quando não estabelecemos para a recursão uma condição de parada de chamada, quando a função tem que parar de se chamar, acontece um processo parecido com o que chamamos de loop infinito quando usamos um for, por exemplo.

 As funções vão se empilhando para serem executadas, e chega uma hora que aquilo explode, então o problema para. O erro que temos é que excedeu a quantidade máxima de processos que estão na pilha para serem executados. É basicamente isso.

 Eu vou deixar um material sobre esse erro no material extra dessa aula. Mas enfim, tivemos um erro de stack overflow.

 Vamos ver o que fazemos então para corrigir isso. Para entendermos o que está acontecendo e porque eu falei que não demos condição de parada para a recursão, eu vou colocar um console.log na primeira linha dentro da função busca.

 Eu vou pedir para esse console passar o que está chegando em cada chamada da função busca nos parâmetros “de” e “até”: console.log(‘de, ate’, de, ate);.

 Vamos rodar novamente. Antes de dar o stack error ele foi fazendo várias chamadas e ele começou a colocar na pilha de execução e tentar ficar chamando a função passando os valores de parâmetro “de” 11 e “até” 10.

 Só que se formos ver, o valor de início não pode ser maior do que o valor de fim de um array. Temos que começar sempre num índice que é menor do que o índice onde para, porque estamos indo ordenadamente.

 Agora que já sabemos o que está acontecendo, o que podemos fazer para lidar com esse erro? Voltando no código, o elemento que não existe no caso que tentamos chamar era um elemento maior, ele teria que estar à direita do meio.

 Quando foram feitas as divisões, sempre tentando achar um número maior do que o maior número que existe, foi-se acrescentando um no valor de “de”. Então “de” sempre começava com mais 1, até que o “de” extrapolou o valor de “até”.

 Então podemos pensar que quando isso acontece é que não encontrou o elemento. Então se não encontrou elemento, retorna alguma mensagem só para conseguirmos um retorno de função que faça com que ela pare de ser executada.

 Vamos fazer então da seguinte forma: antes de começarmos o primeiro if que faz as comparações de valores, vamos colocar um if a mais. Eu vou dizer que se “de” for maior do que “até”, eu vou pedir para retornar -1: if (de > ate) { return -1; }. - 1 é o número de índice que o JavaScript costuma retornar nas suas funções de sort quando não encontra nada.

 Então se encontra um índice ele retorna o número do índice. Se não encontra nada que foi buscado retorna -1. Então vamos retornar -1 se “de” for maior do que “até”.

 Vou limpar o console e testar novamente. Agora o console alertou o que estava acontecendo. Estava tentando primeiro de 0 a 10, depois de 6 para 10, depois de 9 para 10, depois de 10 para 10, e ele foi para frente até que “de” ficou maior do que o “até”. E então ele retornou para nós o -1.

 Podemos apagar o console que colocamos de verificação para deixar o código um pouco mais limpo.

 E agora eu acho que a nossa função de busca está completa. O que acabamos de desenvolver é uma busca chamada de busca binária, porque ela sempre divide a lista em duas partes e procura em uma das duas.

 Então divide em duas, procura em uma das duas partes; divide essa parte em mais duas e procura em cada uma delas; divide em mais duas e procura em cada uma delas.

 Dá para perceber que com esse método o computador vai fazer menos operações do que se fosse pesquisando um por um, passando por todos os elementos. Numa lista de mil elementos ele vai fazer mil processamentos, mas com a busca binária vai fazer bem menos. Primeiro vai dividir, vai pegar só 500 elementos; depois vai dividir de novo e assim por diante.

 Nós temos a impressão de que esse algoritmo é melhor, mas vamos ver agora em seguida se realmente ele é melhor e porque.


#### Outros erros da busca binária


Durante a aula, vimos que, se não colocamos a condição de > ate e tentarmos buscar um número inexistente maior do que qualquer um da lista, o resultado será um erro do tipo RangeError: Maximum call stack size exceeded.

Vamos falar um pouco mais sobre este erro em seguida. Mas agora, vamos testar mais dois casos: Um elemento inexistente menor do que qualquer um da lista, e outro inexistente no meio, ou seja, entre os valores da lista.

Valor menor:
Vamos chamar a função passando 1 como valor buscado:


```
console.log(busca(listaLivros, 0, listaLivros.length - 1, 1));

```


Executando o código, temos o seguinte retorno no terminal:


```
/<diretório>/aula-4/busca.js:11
  if (valorBuscado === atual.preco) {
                             ^

TypeError: Cannot read property 'preco' of undefined
```


Ué, não deveríamos ter recebido um erro do tipo rangeError? O que aconteceu de diferente?

Vamos conferir o que a função busca() está recebendo como parâmetro a cada chamada:


``` 
function busca(array, de, ate, valorBuscado) {
 console.log('de, ate', de, ate)
 //restante do código
}
```

E executar novamente:

```
de, ate 0 10
de, ate 0 4
de, ate 0 1
de, ate 0 -1
```


No caso de valores menores, o código do algoritmo chama a função busca() passando sempre o valor do parâmetro ate diminuindo um número:

```
 if (valorBuscado < atual.preco) {
   return busca(array, de, meio - 1, valorBuscado);
 }
```

Quando o valor atinge -1, que não é um valor válido de índice de array, o resultado de atual.preco retornará undefined.

Valor inexistente no meio do array
Vamos chamar a função passando 36 como valor buscado. Não é menor do que todos nem maior do que todos, porém não existe nenhum objeto com esse valor no array:

```
console.log(busca(listaLivros, 0, listaLivros.length - 1, 36));
```


Executando o código, temos o seguinte retorno no terminal:


```
RangeError: Maximum call stack size exceeded
```


Dessa vez, voltamos a receber o rangeError. Observando o `console.log(‘de, ate’, de, ate), os valores finais retornados são:

```
de, ate 8 7
de, ate 8 7
de, ate 8 7
de, ate 8 7
```


Até atingir call stack size exceeded, da mesma forma que ocorreu quando passamos o valor de 60, maior do que o maior elemento do array.


#### Maximum call stack size



Vamos ver um pouco mais a fundo o que significa o erro RangeError: Maximum call stack size exceeded.

A pilha de chamadas
Em programação, uma pilha é uma estrutura de dados onde o último item adicionado é o primeiro a ser removido - como uma pilha de livros no mundo real, por exemplo. Também nos referimos como pilha (ou stack) a estrutura onde estão “empilhados” os processos que estão sendo executados em um programa.

Nem todo interpretador ou linguagem de programação lida da mesma forma com os processos que devem ser executados por um programa. O NodeJS trabalha com o paradigma de programação orientada a eventos (event driven programming), e o gerenciamento dos processos ocorre através do que chamamos de loop de eventos.

Não vamos entrar em detalhes aqui sobre como ocorrem a entrada e a saída de processos deste loop e a forma como o Node trabalha com threads e programação assíncrona - são assuntos complexos o suficiente para terem seus próprios cursos. Porém, vale mencionar aqui que, assim como em outras linguagens de programação, o JavaScript também trabalha com pilhas de chamadas. No NodeJS, esta pilha faz parte da estrutura do loop de eventos; quando uma função é chamada por um programa ela entra na stack, ou seja, na pilha de execução, onde apenas um processo é executado por vez e o próximo processo só é executado após a finalização do processo atual.

Esta pilha tem uma quantidade limitada de processos que podem ser empilhados (o que depende de muitos fatores, como memória disponível, arquitetura, etc); caso o interpretador não consiga limpar a pilha, ou seja, executar e finalizar os processos/funções que estão empilhados, ao atingir o limite o programa cai no chamado erro de estouro de pilha, também chamado de stack overflow (daí o nome do famoso [fórum de programação](https://stackoverflow.com/)).

Um dos motivos mais comuns para o estouro de pilha são justamente as chamadas recursivas onde o caso base (como vimos na atividade “Para Saber Mais” da aula 2) não existe ou não foi definido da forma correta. Sem o caso base, as funções recursivas não param de ser chamadas e vão se empilhando na pilha de chamadas, até que não haja mais recursos para processar o programa.

No caso do exemplo visto durante a aula, o NodeJS retorna o erro RangeError: Maximum call stack size exceeded, ou “tamanho máximo da pilha de chamadas excedido” e encerra a execução.

Por isso, é muito importante sempre testar as funções recursivas e definir quando interromper a recursividade.



### 9.10 Análise dos Algoritmos



#### Analise da Busca



Algoritmo de crescimento linear --> de um em um da lista


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/52db1371-b0e5-4ed1-ae1c-624ae2f54be6)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/3c3cd16b-03f4-41e3-b579-e220cd4bbb7d)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/0598bf13-edb8-4e48-8d50-b0ad67b3eaa7)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/069da77b-fb02-4ae8-b52a-f238c0dbf404)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/b26bea0f-0ee4-4497-8ae9-d00d64aea5ad)


log na base 2


o numero de operações cresce de acordo com o log de n.


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/34963a50-3842-4499-826d-4e7d9e365782)


![image](https://github.com/FlavianaFXT/algoritmos-js-II/assets/113718720/f1d9dafe-e434-4545-ac72-bb706df18454)


Quando buscamos algo em uma lista utilizando uma busca linear, o programa tem que percorrer todos os elementos da lista até encontrar o que queremos.

 Claro que o elemento buscado pode, por exemplo, estar na primeira posição ou ser uma das primeiras posições.

 Mas quando estamos pensando em cálculo de complexidade de algoritmo isso é meio que irrelevante. Não podemos levar isso em consideração, mesmo porque o elemento pode não existir na lista.

 E se o elemento não existe na lista o programa só vai retornar essa informação depois que passar por todos os elementos, do índice 0 até o último índice, não importa se for uma lista de 10, mil, 10 mil ou 100 mil elementos. Então numa lista de 100 mil elementos são 100 mil operações; numa lista de 20 mil elementos, 20 mil operações.

 Esse algoritmo que pula de elemento em elemento nós dizemos que é um algoritmo de crescimento linear, porque ele cresce em complexidade numa relação direta com a quantidade de elementos que tem na lista. Nós veremos isso num gráfico daqui a pouco.

E a busca binária que acabamos de fazer? Vamos ver como ela funciona. Na busca binária nós pegamos um array, dividimos em dois e localizamos se está para a esquerda ou para a direita do meio. E nessa única operação já descartamos metade de uma lista.

 Então numa lista de mil elementos já descartamos de uma vez só 500 elementos. No caso da nossa lista de 11 elementos, vai dividir no meio e descartar de uma vez seis elementos.

 E vamos, por exemplo, continuar buscando o elemento que está no índice 8, o nono elemento, de valor 40. Começamos dividindo no índice 5, o sexto elemento. Nessa já jogamos todos os seis da esquerda para fora.

 Na próxima vez que formos executar esse algoritmo nossa lista já diminuiu. Dividimos em dois elementos para um lado, três elementos para o outro. Já cortou mais dois e deixou os três da direita.

 Na próxima vez teremos só três elementos para dividir em um de um lado e dois do outro. E nessa já podemos fechar esse algoritmo, porque o elemento buscado já foi encontrado, ele é o único elemento que sobrou do lado dele.

Então vamos colocar isso de uma outra forma. Nós podemos dizer então que para uma lista de dois elementos precisamos de uma operação para encontrar o elemento certo em uma busca linear.

 Se dobrarmos essa lista para quatro elementos, precisamos de duas operações no máximo. Porque a primeira operação vai quebrar o array de quatro elementos em dois, ficando dois para cada lado. E tendo dois para cada lado, com uma operação eu resolvo, lembrando sempre que um dos lados é sempre descartado.

 Dobrando de novo para 8 elementos, agora eu tenho uma operação para dividir em dois arrays de quatro. Um dos arrays de quatro elementos já é descartado e eu fico com um deles. Eu divido ele novamente em dois elementos e uma operação resolve.

 Eu acho então que tem um padrão. Para dois elementos uma operação. Para quatro elementos duas operações. Para oito elementos três operações. Para 16 elementos quatro operações, se seguirmos essa lógica.

 Expressando isso de uma forma matemática podemos dizer que com uma operação conseguimos analisar uma lista de 2 elevado a um elemento. Ou seja, dois elementos.

 Com duas operações, dois elevado a dois elementos, ou seja, quatro elementos. Com três operações, dois elevado a três, então oito elementos. Com quatro operações, dois elevado a quatro, então 16 elementos. Com 10 operações são dois elevado a 10, que dá 1024 elementos.

 Então para uma lista de 1024 elementos, uma busca linear levaria 1024 operações para encontrar um elemento qualquer. E numa busca binária eu só preciso de 10 operações.

 E como chegamos a esse número de quantas operações são necessárias para n elementos, digamos assim? Esse número é um log na base 2. Colocando de outra forma, dizemos que o número que está colocado como potência resulta na quantidade de elementos que estamos buscando.

 Ou seja, 2 elevado a que número dá 1024 elementos? É 10. Então concluímos que o número de operações cresce de acordo com o log desses elementos. Ou seja, é um algoritmo que cresce e expressamos a complexidade desse algoritmo como O log de N.

 Vamos uma olhada no gráfico que já trabalhamos no curso anterior para ver isso colocado com números.



 Então eu tenho na minha planilha já uma coluna com a quantidade de elementos, e eu coloquei n, que é linear. Então eu tenho um elemento e uma operação; 32 elementos e 32 operações.

 E no gráfico está mostrando a linha reta, por isso o nome, de crescimento desse algoritmo, que é a busca linear.

 Agora, para calcular o log de N, vamos passar o valor como sendo A2, que na minha planilha é a casa onde está o número de elementos. E a base é sempre dois, então =log(A2, 2).

 Eu vou usar o recurso de auto completar da planilha. E conseguimos ver no gráfico que o crescimento em complexidade do algoritmo linear é muito maior do que se trabalharmos com um algoritmo de crescimento logarítmico.

 Eu vou diminuir um pouco a quantidade de elementos e deixar só 32 para conseguirmos visualizar melhor o gráfico.

 Conseguimos ver a curva de crescimento de um algoritmo que é O log de n, que cresce em complexidade de uma forma muito mais suave do que um algoritmo linear, que vai percorrer uma lista completa de mil, 2 mil ou 5 mil elementos.

 Então duas coisas que já temos na cabeça: primeiro que é muito importante sabermos como calcular a complexidade de um algoritmo, porque isso impacta na performance do programa que vai utilizar esse algoritmo.

 E vimos também que a busca binária trabalha com um nível de complexidade bem menor do que a busca linear. Ou seja, é muito melhor você fazer 10 operações para uma lista de 1024 elementos do que você fazer 1024 operações para uma lista de 1024 elementos.

E já descobrimos como relacionar o número de base 2 elevado a n e como isso consegue representar a quantidade de elementos que conseguimos trabalhar, de quantas operações para qual quantidade de elementos.

Então agora para uma lista de 5 mil ou de 10 mil elementos, nós conseguimos descobrir quantas operações precisamos fazer através do log.

 Mas lembrando que para a busca binária funcionar o array precisa estar ordenado. Então agora precisamos analisar a complexidade de algoritmo das ordenações que trabalhamos anteriormente durante esse curso.



 #### Analise das Ordenações
 

Já fizemos então a análise do algoritmo de busca linear e busca binária, que foi a que desenvolvemos agora nesse curso.

 Vamos então fazer a análise dos algoritmos de ordenação, merge sort e quick sort, que desenvolvemos durante o curso. Começando pelo merge sort, vamos dar uma olhada no código dele.

 O código que desenvolvemos para o merge sort está em boa parte baseado numa função que chamamos de “ordena”. Essa função “ordena” percorre toda a lista em um loop while, então podemos considerar que os elementos serão percorridos de forma linear, um por um. Ela vai percorrendo, comparando e empurrando para o array de resultados.

 E cada vez que a função merge sort é chamada de forma recursiva, ela divide o array em duas partes cada vez menores. Então o que temos nesse algoritmo é um processamento que acontece de forma linear, ou seja, n, que cresce linearmente; e também um algoritmo que cresce de forma logarítmica, log de n na base 2. Então o que podemos concluir é que nós temos um algoritmo que é n vezes log de n.

 Vamos então comparar isso com um algoritmo de complexidade quadrática, que foi o que vimos no curso anterior, que executa loop dentro de loop, for dentro de for, while dentro de while e etc.

 Na planilha nós temos a coluna com a quantidade de elementos de uma lista, parando em 2048, e uma coluna com o resultado do cálculo de complexidade quadrática, ou seja, for dentro de for e loop dentro de loop, que foi o que concluímos que é a complexidade de algoritmos, por exemplo, como selection sort e insertion sort, usados no curso anterior.

 E podemos ver que, por exemplo, em 2048 elementos temos uma quantidade de operações de 4.194.304, porque fazemos a quantidade de elemento vezes a quantidade de elemento. Então 64 x 64, 128 x 128. Quando isso vai para 2048 é 2048 x 2048.

 E um array de 2000 elementos não é um array tão grande assim. Qualquer escola de tamanho pequeno tem uma quantidade maior até de alunos, só para termos um exemplo de onde uma lista poderia ser aplicada.

 Então a diferença de 4 milhões de operações num selection sort, por exemplo, utilizando um algoritmo de ordenação que cresce de complexidade logarítmica, nós decrescemos essa complexidade de 4 milhões para 22.528 operações, para uma lista de 2048 elementos.

 E nesse caso não é log de n, é n vezes log de n. Já estamos considerando o while, aquele loop que será executado pela função “ordena”.

Algo parecido acontece na estrutura do quick sort. Vamos dar uma olhada no código que desenvolvemos para o quick sort. O quick sort tem uma função que, ao invés de “ordena”, chamamos de “particiona”. A função “particiona” vai dividindo, vai particionando o array e fazendo as trocas de lugar.

E dentro da função “particiona”, de forma parecida com o que temos na função “ordena”, nós temos um while.

Então também podemos dizer que esse while vai ficar percorrendo os elementos, então ele é linear, porque ele precisa comparar cada um dos elementos de um lado para encontrar os maiores ou os menores.

 E enquanto isso a função quick sort vai também funcionar de forma recursiva, chamando a função “particiona”, de forma bem parecida com o que fizemos no merge sort.

 Então podemos dizer que o quick sort também é um algoritmo n vezes log de n. Mas tem dois whiles dentro do while principal. Não teria que ser n quadrático vezes log de n?

 Na verdade os dois whiles de dentro nós não consideramos um loop completo, passando por todos os elementos do array, porque esses whiles que estão dentro do while principal percorrem apenas o trecho necessário. Eles não percorrem o array inteiro. Então ele vai pegar um pedaço, outro pedaço, e assim por diante.

 Então os loops que eles tão fazendo dentro do while principal não são relevantes em termos de quantidade de operações que estão sendo feitas nesse algoritmo.

 Ou seja, assim como o merge sort, o quick sort também é um algoritmo n vezes log de n. Nós utilizamos a notação o vezes log de n. E no gráfico tanto de um quanto do outro a curva de complexidade também é muito menor do que o quadrático.

 Eu vou tirar um pouco de elemento e deixar só 16 elementos na lista para vermos melhor no gráfico como isso ocorre.

 Dá para analisar que só com 16 elementos a diferença de crescimento entre os dois algoritmos é gritante. Passamos de 64 operações para 256 operações para 16 elementos.

 Então se merge sort e quick sort são iguais, como é que comparamos e escolhemos entre eles? Nesse caso, como eles crescem em complexidade basicamente da mesma forma, passamos para alguns outros detalhes, por exemplo, a quantidade de trocas internas que o algoritmo faz.

 Pode ser 2n. 2n e 3n, como vimos no curso anterior, não diferem em muita coisa. Mas num universo de comparação de algoritmo podemos usar como base de comparação.

 Então no final o teste será feito com base em dados do mundo real, lembrando que cada caso é um caso.

 Na média o que se vê é que o quick sort acaba sendo um pouco mais rápido e performático do que o merge sort. Na média ele acaba fazendo menos operações.

Todos os exemplos de algoritmos que vimos nesse curso partem de um princípio que chamamos de dividir para conquistar, onde um problema grande é dividido em partes pequenas. E ao resolver essas partes pequenas resolvemos o problema por inteiro.

 Porque tentar atacar um problema grande de uma vez só, como faz, por exemplo, o selection sort e o insertion sort, é mais lerdo. Vai ter mais operações para serem feitas, isso reflete em mais processamento, e já vimos anteriormente como isso impacta na performance de um programa.

É bom sempre questionarmos qual é o algoritmo que está sendo utilizado para resolver algum problema. Eles resolvem problema de computação, buscar, ordenar etc.

Muitas linguagens de programação já têm os seus métodos de ordenação e de busca implementados. E uma coisa interessante é descobrirmos o que está por trás dos métodos.

 Por exemplo, o JavaScript tem seu próprio método array.sort. Qual é o algoritmo que faz com que o sort do JavaScript funcione? Essa é uma coisa bacana de pesquisarmos e entendermos.

Porque por trás de toda implementação, mesmo dos métodos que as linguagens já trazem prontos para nós, existe um algoritmo.

 E agora que já sabemos melhor como funcionam os conceitos que estão por trás do desenvolvimento de um algoritmo, conseguimos ir atrás e entender melhor como eles funcionam, quais são os melhores para as nossas necessidades e para as necessidades dos nossos projetos.




#### Métodos do JavaScript


No dia a dia do trabalho, é muito comum usarmos métodos nativos - ou seja, aqueles que já são próprios da linguagem e só precisam ser “chamados” como funções - para que nosso código fique mais legível ou então para simplificar o trabalho. Exemplos bem comuns são os métodos sort() e find(), respectivamente usados para ordenação e busca.

O método sort() molda elementos de um array em strings e os ordena em ordem crescente. Vamos ver um exemplo?


```
let numeros = [1, 2, 3, 101, 20, 3, 30, 31, 40];
numeros.sort();
console.log(numeros);

// Saída
// [1, 101, 2, 20, 3, 3, 30, 31, 40]
```


Observe que a saída mostra a classificação dos números um pouco diferente do esperado. Isso ocorre pois o método trata os elementos do array como strings e os coloca em ordem sequencial de acordo com sua posição na [tabela ASCII](https://www.asciitable.com/), onde 20 vem antes de 3.

Para que o sort() funcione de acordo com o esperado, precisamos passar os parâmetros de comparação de forma explícita:


```
var numbers = [4, 2, 5, 1, 3];
numbers.sort(function(a, b) {
  return a - b;
});
console.log(numbers);
// Saída 
//[1, 2, 3, 4, 5]
```

Você pode conferir com detalhes o uso do sort() em JavaScript na documentação do [MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Array/sort).

Indo além do uso do método no dia a dia, já imaginou como esses métodos funcionam “por baixo dos panos”? Não é somente uma palavra para complementar seu código, pois assim como criamos funções, os métodos nativos da linguagem também possuem lógica e algoritmos por trás. Vamos conhecer um pouco mais?

No JavaScript, a forma como o método é implementado depende do motor que faz a interpretação. A partir de cada versão aprovada do JavaScript pelo ECMA, as empresas ou fundações responsáveis pelos navegadores/interpretadores (chamadas de vendors no jargão da área) decidem e fazem a implementação das funcionalidades.

No caso do motor V8, utilizado pelo Chrome/NodeJS, o sort() tem em sua implementação os algoritmos quick sort - ordenação rápida e insertion sort - ordenação por inserção, e funcionam da seguinte maneira:

```
 function QuickSort(a, from, to) {
    var third_index = 0;
    while (true) {
      // Insertion sort is faster for short arrays.
      if (to - from <= 10) {
        InsertionSort(a, from, to);
        return;
      }
```


Por outro lado, no motor SpiderMonkey, utilizado pelo Firefox, o algoritmo utilizado por trás do método sort() é o merge sort, implementado abaixo em C++:

```
JSBool
js::array_sort(JSContext *cx, uintN argc, Value *vp)
{
    jsuint len, newlen, i, undefs;
    size_t elemsize;
    JSString *str;

    Value *argv = JS_ARGV(cx, vp);
    Value fval;
    if (argc > 0 && !argv[0].isUndefined()) {
        if (argv[0].isPrimitive()) {
            JS_ReportErrorNumber(cx, js_GetErrorMessage, NULL, JSMSG_BAD_SORT_ARG);
            return false;
        }
        fval = argv[0];     /* non-default compare function */
    } else {
        fval.setNull();
    }

    JSObject *obj = ToObject(cx, &vp[1]);
    if (!obj)
        return false;
+
−    if (!js_GetLengthProperty(cx, obj, &len))
        return false;
    if (len == 0) {
        vp->setObject(*obj);
        return true;
    }

    /*
     * We need a temporary array of 2 * len Value to hold the array elements
     * and the scratch space for merge sort. Check that its size does not
     * overflow size_t, which would allow for indexing beyond the end of the
     * malloc'd vector.
     */
#if JS_BITS_PER_WORD == 32
    if (size_t(len) > size_t(-1) / (2 * sizeof(Value))) {
        js_ReportAllocationOverflow(cx);
        return false;
    }
```


Esse conhecimento é importante para escolhermos os métodos nativos que aplicamos em nosso código e também para entendermos certos comportamentos dos programas e aplicações ao serem interpretados pelos motores.

Você pode conferir aqui o código-fonte implementado pelo motor [SpiderMonkey](https://hg.mozilla.org/mozilla-central/file/28be8df0deb7/js/src/jsarray.cpp) e pelo motor [V8](https://github.com/v8/v8/blob/fe598532ec1317e8b85343133be9fb708e07bd2e/src/js/array.js#L768).

Bônus: ordenação estável
Algoritmos de ordenação podem ser estáveis ou instáveis. Caso queira começar neste assunto, este tópico do [Stack Overflow](https://pt.stackoverflow.com/questions/188646/o-que-define-um-algoritmo-de-ordena%C3%A7%C3%A3o-est%C3%A1vel) tem informações em português para começar; em seguida você pode conferir os [testes de estabilidade do método array.sort() em diferentes navegadores (em inglês)](https://stackoverflow.com/questions/3026281/what-is-the-stability-of-the-array-sort-method-in-different-browsers).


#### Melhor caso versus pior caso


Durante o desenvolvimento do código do quick sort, comentamos sobre o pior caso de execução de um algoritmo.

Em algoritmos, os termos melhor caso e pior caso se referem à quantidade de recursos a ser utilizado na execução, que pode ser tempo de execução ou memória.

Uma maneira adotada para mensurar a eficiência dos algoritmos, tendo em vista tempo de execução e espaço de memória, é por meio da notação Big O, que realiza a comparação desses dois parâmetros.

Lembrando que a notação [Big O](https://estevestoni.medium.com/iniciando-com-a-nota%C3%A7%C3%A3o-big-o-be996fa3b47b) se refere a uma classificação de algoritmos de acordo com o tempo de execução, à medida em que aumenta a quantidade de dados a serem manipulados e a quantidade de memória exigida.

Dessa forma, teremos o melhor caso de algoritmo quando ele apresenta a mesma quantidade de tempo para executar, independente do tamanho da entrada. E um pior caso quando se tem um maior tempo de execução considerando todas as possíveis entradas.

Exemplo de Big O em algoritmos de ordenação:

```
Algoritmo	estrutura	Complex. tempo: melhor caso	Complex. tempo: pior caso	Complex. espaço: pior caso
Quick Sort	Array	O(n log(n))	O(n²)	O(n log(n))
Merge Sort	Array	O(n log(n))	O(n log(n))	O(n)
Heap Sort	Array	O(n log(n))	O(n log(n))	O(1)
Smooth Sort	Array	O(n)	O(n log(n))	O(1)
Bubble Sort	Array	O(n)	O(n²)	O(1)
Insertion Sort	Array	O(n)	O(n²)	O(1)
Selection Sort	Array	O(n²)	O(n²)	O(1)
```

Onde:

O(1): notação de Big O que representa um algoritmo que é executado em tempo constante.

O(n): algoritmo que é executado em tempo linear, ou seja, as execuções aumentam de acordo com as entradas - como a busca linear.

O(n log(n)): representa um algoritmo que reduz pela metade uma lista a cada vez que é executado - como o merge sort e o quick sort.

O(n²): algoritmo com o tempo quadrático que por sua vez, significa que assim que o número de elementos na entrada aumenta, as execuções aumentam quadraticamente. Por isso, devemos evitar códigos com essa notação de Big O, pois o número de operações aumenta significativamente a cada entrada - como o selection sort e o insertion sort.


#### Logaritmo binário


Em computação sempre é utilizado o logaritmo com base 2 (e, consequentemente, o inverso é a potência de 2). Assim, log n representa de forma abreviada log2 n, ou seja, log de n na base 2.

Esta característica está ligada ao sistema numérico utilizado pelos computadores: o sistema binário (ou de base 2), onde todos os valores são representados pelos números 0 e 1.

Assim, sempre que trabalharmos com valores O(log n), estamos nos referindo a base 2.


## Projeto Final do Curso [AQUI](https://github.com/alura-cursos/2360-algoritmos-js-II/tree/aula-4)


## 9.11 CONCLUSÃO ALGORITMOS

Aprendemos a fazer a análise assintótica do algoritmo de busca binária e por que este é considerado um algoritmo de complexidade logarítmica, em comparação com a busca linear que é um algoritmo de complexidade linear;
Fizemos a análise assintótica dos algoritmos de ordenação quick sort e merge sort e analisamos o código para entendermos por que são considerados algoritmos de complexidade linear-logarítmica;
E o que significa, em termos de performance, a diferença entre algoritmos de crescimento linear, quadrático e logarítmico.

# EXERCICIOS

```
1 - - Explicação do exercício: Adivinhe o número.
O usuário tem que adivinhar um número inteiro aleatório entre 0 e 50.

Se ele acertou, então dar os parabéns e encerrar.
Se for um número baixo, responder é maior
Se for um número alto, responder que é menor.

Extra: o usuário tem o limite de 5 tentativas para acertar o número

OBS: usar este código para gerar um número aleatório
Math.floor(Math.random()*(50 - 0 + 1));
```


```
2 - Explicação do exercício: Escrever um programa que receba um e-mail e uma senha e só permita que o login seja feito quando o e-mail for teste@reprograma.com E a senha seja teste123, caso um deles esteja errado escrever uma mensagem de erro e perguntar e-mail e senha novamente até o usuário acertar.
EMAIL E SENHA PRECISAM ESTAR CORRETOS email E senha digitados estão iguais a teste@reprograma.com e teste123

DADOS CERTOS -> LOGIN DADOS ERRADOS -> ERRO

ESTRUTURA DE DECISAO -> IF/ELSE (SE/SENAO)

PASSOS PARA RESOLVER O EXERCICIO:

receber e guardar um email e uma senha OK
guardar email correto e senha correta OK
comparação de email e senha para verificar se pode fazer login (se email e senha certos, fazer login, senão dar mensagem de erro)
repetir ações ENQUANTO email e senha incorretos
```

```
3 - Faça uma função que recebe o preço de um produto e o percentual de desconto a ser dado no produto e retorne o valor do produto com desconto.
```

```
4 - Criar uma função que receba a idade de uma pessoa e diga quais filmes aquela pessoa pode assistir. Use como base o seguinte objeto:

let filmes = [ { nome: "Deadpool", classificacaoEtaria: 18 }, { nome: "Your Name", classificacaoEtaria: 0 }, { nome: "Kill Bill", classificacaoEtaria: 18 }, { nome: "Shrek", classificacaoEtaria: 0 }, { nome: "Matrix ", classificacaoEtaria: 14 }, { nome: "Você nem imagina", classificacaoEtaria: 12 }, { nome: "Brilho eterno de uma mente sem lembranças", classificacaoEtaria: 14 }, { nome: "Scott Pilgrim contra o mundo", classificacaoEtaria: 12 }, { nome: "Capitão Fantástico", classificacaoEtaria: 14 }, { nome: "El Camino", classificacaoEtaria: 16 }, { nome: "Parasita", classificacaoEtaria: 16 }, { nome: "Star Wars: o retorno do jedi", classificacaoEtaria: 0 }, { nome: "Red: crescer é uma fera", classificacaoEtaria: 0 }, { nome: "Ninja Assassino", classificacaoEtaria: 18 }, ]
```


# LINKS UTEIS:


- [Como formatar número com JavaScript](https://www.alura.com.br/artigos/formatando-numeros-no-javascript?_gl=1*1j0vrgf*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwOTczMTQ4NS4zNS4xLjE3MDk3MzM0NTAuMC4wLjA.*_fplc*UEg3RkVXQTFWQXpOU3BGdUdoWkpOWDR6Qmk2QkJFbmR4RXpEdjl1OVh6Qm1DZCUyRnRwVDJ3UzZ4UDZja0NwWjVJWEhta3JaUUZuanZHcDRXa3UwUXNOJTJCeGtsME5Ca0g0dWszU1pFRFIlMkJITVU0MHNFZ2VGR3E1JTJCanlkZU5nYXclM0QlM0Q.)
- [Como ordenar uma sequência de números no JavaScript](https://www.alura.com.br/artigos/ordenacao-de-numeros-no-javascript-nao-funciona?_gl=1*164k246*_ga*MTAyMjIzNjI2OC4xNzAxODc3NTU5*_ga_1EPWSW3PCS*MTcwOTczMTQ4NS4zNS4xLjE3MDk3MzM0NzkuMC4wLjA.*_fplc*UEg3RkVXQTFWQXpOU3BGdUdoWkpOWDR6Qmk2QkJFbmR4RXpEdjl1OVh6Qm1DZCUyRnRwVDJ3UzZ4UDZja0NwWjVJWEhta3JaUUZuanZHcDRXa3UwUXNOJTJCeGtsME5Ca0g0dWszU1pFRFIlMkJITVU0MHNFZ2VGR3E1JTJCanlkZU5nYXclM0QlM0Q.)
- [MDN](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
- [W3Schools](https://www.w3schools.com/js/default.asp)
- [Lorem Ipsum](https://www.lipsum.com/feed/html)
- [Lorem Ipsum](https://www.lipsum.com/feed/html)
- [Objetos](https://developer.mozilla.org/pt-BR/docs/Learn/JavaScript/Objects/Basics)
- [Funções](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Functions)
- [For](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/for)
- [While](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/while)
- [Arrow Function](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Functions/Arrow_functions)
- [Callbacks](https://www.freecodecamp.org/news/javascript-callback-functions-what-are-callbacks-in-js-and-how-to-use-them/)

# Plataformas de estudos

- [URI Online Judge](https://www.urionlinejudge.com.br/judge/pt/login?redirect=%2Fpt)
- [FreeCodeCamp](https://www.freecodecamp.org/)
- [KhanAcademy](https://www.khanacademy.org/computing/computer-programming)














