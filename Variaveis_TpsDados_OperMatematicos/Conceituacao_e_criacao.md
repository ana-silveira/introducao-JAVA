### Conceituação e criação de variáveis
- Objetivos:
-- Entender o que são variáveis
-- Saber como criar variáveis

- Conceito de *variável*: "Um espaço na memória do computador onde se pode guardar valores". É um espaço de reserva que a gente cria no computador visando guardar um valor na memória. 
- Existem 4 tipos:
-- Instância: pertence ao objeto 
-- Classe: classe
-- Local: dentro de métodos (Criaremos nossas variáveis iniciais dentro do método "Main")
-- Parâmetro: na assinatura do método

- Padrão de definição: <?visibilidade?><?modificador?> tipo nome<?=valorInicial?>;
---- O que está entre "?" significa que podemos criar variáveis sem prover tais informações. Isso vai depender do tipo da variável e da sua necessidade.
---- V: "public", "protected" e "private" (muito relacionado a orientação ao objeto)
---- M: "static" (rel. a orientação ao objeto) e "final" (variável é constante, não muda)
---- T: Tipo de dado (**É obrigatório; sempre precisa ser informado. Por causa disso a linguagem JAVA se caracteriza como "TIPADA"**)
---- N: Nome que é fornecido a variável para saber para quê ela serve.
---- VI: um valor inicial caso seja desejado

- Convenções e regras para os nomes das variáveis;

-- Não podem começar com números;
-- Não inserir caracteres especiais;
-- Embora permitidos, $ e _ devem ser evitados;
-- São case-sensitives: JAVA reconhece e diferencia letras maiúsculas e minúsculas.
-- Não inserir espaços nos nomes das variáveis. 
-- Existe uma lista de palavras que não podem ser utilizadas para nomear variáveis (palavras reservadas).

-- Sempre começar com letra minúscula;
-- Nomes expressivos, claros e objetivos;
-- Notação camelo (deixar em maiuscula a 1a letra de cada palavra que compõe o nome da variável, com exceção da 1a);
-- Quando constante (final), o nome da variável é todo em maiúscula e separada por "_". Ex: --> int **final** NUMERO_TENTATIVAS = 5

# #Quando todo mundo segue as boas práticas, o código é facilmente interpretado por todos!#






