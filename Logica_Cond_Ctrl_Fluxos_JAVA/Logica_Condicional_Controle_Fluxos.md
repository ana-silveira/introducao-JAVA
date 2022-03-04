# Operadores lógicos e relacionais, controle de fluxos e Blocos

**Objetivo do curso**: Possibilitar a compreensão de operadores lógicos e relacionais, além de estruturas de controle de fluxo e blocos. 

Percurso: 
- Aula 1: Operadores relacionais
- Aula 2: Operadores lógicos
- Aula 3: Controle de fluxo
- Aula 4: Blocos

---------------
Aula 1: Lógica Condicional e Controle de Fluxos em Java

1. Objetivos:
- Entender o que são operadores relacionais;
- Simbologia utilizada
- Como utilizar os operadores relacionais;

Conteito: São simbolos especiais capazes de realizar comparações entre determinados operandos, e , em seguida, retornar um resultado. 
- Tipo: 
-- Similaridade: 
    -- Igualdade (==) : Determina se um operando é igual ao outro;
    -- Diferença (!=) : Determina se um operando não é igual ao outro. 
    * Tomar cuidado para não deixar de colocar o duplo = quando se tratar se um caso de similaridade, para não haver erro de execução no código e o sentido mudar para atribuição.
-- Tamanho: maior (>), maior igual (>=), menor(<), menor igual(<=)

------------------------

Operadores Lógicos:

-  Objetivos:
--  1. Entender o que são operadores lógicos;
--  2. Saber como utilizá-los

- Conceito: São simbolos especiais capazes de realizar comparações lógicas entre operandos lógicos ou expressões e, em seguida, retornar um resultado. ---> Nesse caso, aplica-se a expressões ou operadores que retornem valores lógicos ===> true ou false! Ou seja, operadores lógicos são mais restritos quanto ao uso. 

- Tipos: Conjunção, Disjunção, Disjunção exclusiva e Negação

1. Conjunção: Operação lógica que só é verdadeira quando ambos os operandos ou expressões envolvidas são verdadeiras. Simbologia: && / Terminologia: and (e);
2. Disjunção: Operação que só é falsa quando ambos os operandos ou expressões envolvidas são falsas. Simbologia: || / Terminologia: or (ou)
3. Disjunção exclusiva: Operação que só é verdade quando ambos os operandos ou expressões são opostos. Simbologia: ^ / Terminologia: xor
4. Negação: Operação que inverte o valor lógico de um operando ou expressão. Simbologia: ! / Terminologia: inversão. 

Curiosidades: Operadores Bitwise : & e | --> Vai mexer com bits, de números bits. Eles não são operadores do tipo lógico. 
Operadores shift: ~, >>, >>>, <<     ---> uso raríssimo. 

Boas práticas: 
- Crie variáveis auxiliares para guardar resultados intermediários. Linhas menores facilitam o entendimento do código e a sua manutenção. 

        (salarioMensal < mediaSalario) && (quantidadeDependentes >= mediaDependentes) pode ser (salarioBaixo) && (muitosDependentes)
        boolean recebeAuxilio = (salarioBaixo) && (muitosDependentes); 

-------------------------

Controle de FLuxo: 

Objetivos:
1. Entender o que são estruturas de controle de fluxo;
2. Saber como usar cada uma.

Conceito: São estruturas com capacidade de direcionar o fluxo de execução do código. 
Se nenhuma dessas estruturas fosse utilizada, o código seria executado de cima para baixo, da esquerda para direita; Porém, tais estruturas são importantes para direcionar o código para que funcione numa ordem / fluxo diferente, como: O código executar uma parte e outra parte, não; executar um trecho repetidas vezes, abortar pedaços do código ou ele todo, etc. Ou seja, com as estruturas de fluxo a gente manipula a forma como o código vai executar. 

Tipos de estruturas de controle de fluxo: 
- Decisão: if, if-else, if-else-if, switch, e operador ternário;
-- Estrutura que avalia uma condição booleana ou variável para direcionar o fluxo de execução. 
- Repetição: for, while, do while.
- Interrupção: break, continue, return. 

Obs: Aqui, somente estruturas de decisão serão abordadas. 

Boas práticas: 
- Switch é para valores exatos e if é para expressões booleanas;
- Evitar usar o default do switch para cases genéricos; 
- Evitar o desfecho 'flecha' dos If's
- Evitar muitos if's aninhados
- Usar a boa prática da aula 2 para diminuir o tamanho do if. 


-------------------

Aula 4: Blocos

Objetivos: 
1. Entender o que são Blocos;
2. Tipos de blocos;
3. Saber como utilizar blocos;

Conceito: Blocos são um grupo de 0 (zero) ou mais códigos que trabalham em conjunto para executar uma operação. Embora seja válido e possível criar um bloco de 0 códigos, não é usual. O bloco normalmente tem, pelo menos, 1 linha a ser executada. 

Tipos:
Locais: dentro de métodos. 
Estáticos: dentro de classes;
Intâncias: dentro de classes;

Criação: Tudo que fica entre as chaves {} é um bloco de execução. Porém, havendo somente 1 linha de execução, não existe obrigatoriedade de abrir e fechar as chaves. 







