03/02/2022

# Documentação Java

- Comentários em Linha
-- São feitos com duas barras no início do comentário "//"
    Ex: // Aqui está um comentário. 

- Comentários em bloco
-- São iniciados por uma barra (/) seguida de 2 asteriscos, e finalizados por um asterisco e uma barra na linha seguinte ao final do comentário."*/".
    Ex: /**
Aqui está um comentário. 
Aqui está outro comentário. 
*/

- O que é o JAVAdoc:
-- É uma ferramenta de documentação no formato HTML, que se baseia nos comentários do código fonte. Esses comentários do código-fonte precisam conter tags para que a documentação fique legível. 
-- O JAVAdoc é basicamente uma ferramenta que lê essas tags e traduz num HTML em que outros desenvolvedores conseguem acessar essa página e entender o que significa cada classe, método e atributo do código fonte.

- Tags do JAVAdoc: 
-- Ela é sempre composta por @ + nome da tag. 
-- Tipos de tags para que a ferramenta consiga processar a página HTML:
**@autor**: Especifica o autor da classe ou do método;
**@deprecated**: Identifica classes ou métodos obsoletos;
**@link**: Possibilita a definição de um link para um outro documento local ou remoto através de uma urL;
**@param**: Descreve um parâmetro que será passado a um método;
**@return**: Descreve qual o tipo de retorno de um método.
**@see**: Associa a outras classes ou métodos;
**@since**: Descreve desde quando uma classe ou método foi adicionado;
**@throws**: Descreve os tipos de exceções que podem ser lançadas por um método;
**@version**: Descreve a versão da classe ou método.

    Ex: 
    
    import java.math.BigDecimal;
    /**
     @author Ana Carolina
     @version 1.0.0
     @see BigDecimal
     @since Release 1.0.0
    */
    
    public class Order {
        // Comentários em linha não são levados pra o JAVAdoc. 
        private final String code;
        private final BigDecimal totalValue;
        /**
        Construtor de classe
        @param code - Código do pedido
        @param totalValue - Valor total do pedido
        @return - Valor total do pedido com as taxas
        @throws - *RunTimeException* Se o valor do pedido for negativo
        */
        
    }
 
Obs: O arquivo index.html poderá ser encontrado dentro do package.
    
    