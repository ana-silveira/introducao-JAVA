#Tipos de Dados

**Objetivos**:
1. Entender o que são tipos de dados;
2. Saber como e quando usar cada um

**Conceito**: "São valores e consequentemente operações que as variáveis podem assumir e sofrer, respectivamente". 
- O "Tipo de Dado" é um conjunto de 3 coisas: 
-- Valor em si daquele tipo;
-- Os conjuntos de valores que ele pode assumir;
-- As operações que podem ser realizadas em cima desses valores. 

**Tipificação**: Pode variar de acordo com a linguagem de programação. Existem duas preocupações que a linguagem deve ter: 
1. Se ela será Estática (forte) ou Dinâmica (fraca)
-- Tipificação Estática é quando uma linguagem obriga vc a definir o tipo da variável já no momento da criação dela. Durante o processo de compilação ele já vai detectar qual é o tipo daquela variável e sempre será aquele tipo, não vai mudar.  Já na tipificação dinâmica, não é obrigatório tipificar a variável no momento da sua criação. Durante a execução da aplicação, a linguagem vai detectar, inferir o valor que está ali dentro e assumir que a variável é de um determinado tipo. É considerado "fraco". Obs: Ver sobre linguagens compiladas e interpretadas. 
2. Se ela será Primitiva ou Composta
-- "Primitiva": São valores numéricos, textuais, os mais básicos que a maioria das linguagens costumam prover. 
-- "Composto" Está muito ligado a Orientação a objeto, instruct. etc. Dados do tipo composto são heterogêneos, possuindo dados primitivos e/ou outros compostos. Ex: C, Instruct. 

**Opções de tipos:**
- **textual**: Caracteres, palavras, texto em geral
-- char: caracteres de 16-bit unicode --> char c = 'T'; *ou* char c = '\u0084'; Trabalha-se caractere por caractere! 
-- String: um tipo "especial" --> String s = "T"; (reparar nas aspas duplas). 
######### Apesar de string ser um tipo de dado relacionado a orientação a objeto, um dado do tipo composto, é muito dificil escrever textos utilizando somente o tipo de dado "char"; O tipo string foi se 'primitivando' devido a necessidade inerente de criar e utilizar muito tipo de dado textual. 
- **numeral**: numeros que podem ser inteiros ou fracionados (reais). A depender da quant de bits que cada numero tiver, vai influenciar na capacidade de armazenamento.
-- byte: 128 até 127 --> byte b = 15;
-- short: -32.768 até 32.767 --> short s = -15.785;
-- int: -2.147.483.648 até 2.147.483.647 --> int i = 8.515.785 ; 
-- long: -9.223.372.036.854.775.808 até 9.223.372.036.854.775.807 --> long l = 5938515785L;
-- float: +- 3.40282347E+38F  --> float f = 3,14...(f);
-- double: +- 1,79769313486231570E+308 --> double d = 3.14...(d);
######## A capacidade de armazenamento aumenta desde o byte até o double!
- **lógico**: Não tem tamanho como os números; Informa se variável é do tipo "verdadeira" ou "falsa".
-- boolean: true e false --> boolean s = false;
- **Objetos**: Relacionados a orientação. Obs: Orientação orientada a objetos não será abordada neste curso. 

** Obs: ** Todo tipo de dado tem seu 'valor default"; É um valor inicial possuido pela variavel de um tipo de dado,  mesmo que uma variável ainda não possua seu valor definido. 
- 