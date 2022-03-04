Estruturas de Repetição e Arrays em JAVA

Objetivoss:
1. Conhecer as estruturas de repetição;
2. Arrays na linguagem JAVA;
3. Estrutura for-each

Percurso:
1. Comand While;
2. Comando do-while;
3. Comando for;
4. Controle de repetição: break e continue;
5. Arrays
6. Comando for-each

Visão Geral: 

-->  O real poder dos computadores está na sua habilidade para repetir uma operação ou uma série de operações várias vezes;
--> Cada repetição é chamada ** laço** (loop), e é um dos conceitos básicos da programação estruturada. 
--> Uma estrutura de repetição permite que uma sequência de comandos seja executada repetidamente, caso determinadas condições sejam satisfeitas. 
--> Essas condições são representadas por expressões lógicas. 
--> As estruturas de repetição são classificadas como:
        Repetição com teste no início (while)
        Repetição com teste no final (do-while)
        Repetição contada (for)
--> O comando *break* é utilizado para terminar de forma abrupta uma repetição. 
--> Quando comando *continue* é executado, os comandos restantes da repetição são ignorados e o programa volta a testar novamente, ou não. Além disso, diferente do break, o continue só pode ser utilizado dentro de uma estrutura de repetição. Obs: O continue é pouquissimo utilizado....

While: A **expressão** é avaliada como True ou False; Se True, cai na sentença e volta para a expressão ciclicamente até que o valor seja False e finalize a aplicação. A sentença vem depois da expressão e pode nunca ser executada!

Do-while: Iniciado o programa, a sentença será executada antes da expressão; Expressão executada, ela sendo true repete a sentença e cai novamente na expressão, até que o valor dessa expressão seja false e o programa finalize. Ou seja, a sentença sempre será executada. 

For:  O programa é inicializado e haverá execução de um teste que, se false, encerrará o programa; se true, executará a sentença E ocorrerá uma atualização no teste, que vai rodar novamente até resposta "false". Essa atualização pode acontecer tampbém no while e no do-while mas no for é obrigatório. 

Operadores de Incremendo e Decremento:
- Pré fixados: ++ numero => número = numero + 1 -> (retorne número)
               -- numero => numero = numero -1 -> (retorne número)
- Pós fixados: numero ++ => (retorne número) ->  numero = numero + 1 
               número -- => (retorne número) -> numero = numero -1 
** Os pós fixados são os mais utilizados. 

Operações aritméticas
-- numero += K ( numero = numero + K);
-- numero -= K ( numero = numero - K);
-- numero *= K (numero = numero * K);
-- numero /= K (numero = numero / k);

Arrays: 
- Um array é um objeto utilizado para armazenar sequencialmente dados do mesmo tipo. 
- A ordem dos dados inseridos no array importa! E só se pode inserir dados do mesmo tipo. Ex: Não pode inserir dados do tipo int (ex: idade) e double(ex: altura) dentro da mesma Array; Precisa haver 2 arrays diferentes.
- Uma vez criado, o array permanece com o mesmo tamanho. Preciso dizer qual é numero de posições que essa array pode ter. 
- Existem arrays **unidimensionais**(cada array é uma linha) e **multidimensionais** (linha e coluna). 


RESUMO: 
1. Pra que serve a estrutura de repetição: Eu vou ter determinada sequência de comandos que eu quero que se repita; para que eu possa controlar se vai repetir ou não essa sequencia de comandos, terei uma expressão, um teste, que vai dizer se é V ou F, se vai executar e quantas vezes vai executar a sequencia de comandos. 
2. Array: É uma estrutura que armazena varios elementos dentro de uma mesma variável.Eu preciso dizer quantos elementos ela pode ter.





