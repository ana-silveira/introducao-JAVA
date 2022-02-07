03/02/2022
# Contextualização de uso do JAVA 11

- Palavras reservadas: Existe uma lista de palavras que não podem ser utilizadas para definição do nome de classes, atributos ou métodos. 

- Declarações de classes: Estrutura básica de uma classe é formada pelo *modificador de acesso* (Ex: public class) e pelo nome da palavra representando um objeto do mundo real (sempre começando com letra maiuscula - ex: Order )
    -- Estrutura com classes e atributos

        public class Order {
        // atributos
        private final String code;
        private final BigDecimal totalValue;

        // metodos
        public BigDecimal calculateFee() {
            }
        }
    
    -- Estrutura completa de uma classe:
    
        package com.dio.base;
        import java.math.BigDecimal;
        public class Order {
            private final String code;
            private final BigDecimal totalValue;
            
            public Order(String code, BigDecimal totalValue) {
                this.code = code;
                this.totalValue = totalValue;
            }
            public BigDecimal calculateFee(){
                return this.totalValue.multiply(new BigDecimal("0.99"));
            }
        }
    
- Modificadores de acesso
-- Tipos de modificadores:
**public**: Qualquer classe de qualquer pacote poderá acessar o atributo ou método.
**protected**: Qualquer classe definida no mesmo pacote ou subclasse poderá acessar o atributo ou método.
Sem modificador: Apenas classes definidas pelo mesmo pacote podem ter acesso a aquele atributo ou método.
**private**: Apenas a própria classe tem acesso a aqueles atributos ou métodos. 

- Métodos
-- São funções que determinam o comportamento de uma classe. 
-- Tipos de métodos: 
**Métodos construtores**: Definem como uma classe será instanciada "construída"
**Métodos comuns**: Definem comportamentos que podem ou não estar atribuídos às regras de negócio. Ex: calcular taxas de um pedido etc. 

- Estruturas de condição
-- São responsáveis por fazer o desvio do fluxo de execução de um código de acordo com uma dada condição. No JAVA existem duas estruturas de condição:
**if - else**: "Se o valor do pedido for maior que 100, a taxa é X; Senão, a taxa será Y."
**Switch - case**: "Se o valor do pedido for até 100, a taxa é X; Se o valor for até 200, a taxa é Y; Caso contrário (se não atende a essas condições), o valor total será somente o valor do pedido, sem taxas."

- Estruturas de repetição
-- São responsáveis por executar repetidamente uma instrução ou bloco de instruções até que uma condição seja satisfeita. 
-- Tipos de estruturas de repetição:
**while**: Determinado comando acontece - enquanto - a condição não é satisfeita. 
**do - while**:  
**for**: 
**enhanced for**:

