
Objetivos: Possibilitar que o aluno compreenda o que é um método, como criá-lo e utilizá-lo. 

Percurso: Criação / Sobrecarga / Retornos

---------------------------------------------------

Aula 1: Criação de Métodos -

1. Entender o que é um método;
2. Saber como definir e utilizar métodos; 
3. Aplicar boas práticas em sua criação e uso. 

Conceito: Método é uma porção de código (sub-rotina) que é disponibilizada por uma classe. Este é executado quando é feita uma requisição a ele. Métodos são responsáveis por definir e realizar um determinado comportamento. 

Todo método é criado DENTRO de uma classe!
Ele precisa ser requisitado, ou seja, chamado para ser executado; Não executa por si, só. 
Tudo que queremos que aconteça estará dentro dos métodos!

Como devemos CRIAR um método? 
Padrão de definição:  <?visibilidade?><?tipo?><?modificador?> retorno nome (<?parâmetros?>) <?exceções?> corpo. 
-> Entre ?? é opcional; Retorno, nome e corpo são obrigatórios. 

Sendo: 
**<?visibilidade?>**: "public", "protected" ou "private"
<?tipo?>: "concreto" ou "abstrato"
<?modificador?>: "static" ou "final"
**retorno**: tipo de dado ou "void"(vazio - o método vai executar e no final não retornará nada)
**nome**: nome que é fornecido ao método
**<?parâmetros?>**: parâmetros que pode receber
<?exceções?>: Exceções que pode lançar
**corpo**: código que possui ou vazio. 

Ex: public String getNome( ) {...}
public int verificarDistancia(int coordenada1, int coordenada2) { }
public abstract void executar ; (aqui temos o corpo {} = vazio)

**public static R N (P) {}** ---> Forma mais utilizada no curso. 

Utilização: Passa-se uma mensagem através de uma classe ou objeto. 

    nome_da_classe.nome_do_metodo(); ou nome_da_classe.nome_do_metodo(...);
    nome_do_objeto.nome_do_metodo(); ou nome_do_objeto.nome_do_metodo(...);

Ex: Math.random(); ou Math.sqrt(4);  ---> Chamando o método a partir da classe (com parâmetro ou não)
usuario.getEmail(); ou usuario.alterarEndereco(Endereco) ---> Chamando o método a partir do objeto (com parâmetro ou não)
*Na escrita, o objeto se diferencia da classe pela letra inicial - objetos tem o nome com 1a letra minúscula (usuario), e a classe tem letra maiúscula (Math)

---------------------------------------------

Conceitos inerentes aos métodos e boas práticas na sua criação

Particularidades: 
- Assinatura: nome + parametros
--  Metodo:

        public double calcularTotalVenda (double precoItem1, double precoItem2, double precoItem3) {
        ...}

    -- Assinatura:

      calcularTotalVenda (double precoItem1, double precoItem2, double precoItem3)

- Construtor e Destrutor: são métodos especiais usados na Orientação a objetos. 
- Mensagem> é o ato de solicitar ao método que o mesmo execute. Esta pode ser direcionada a um objeto ou a uma classe. 
- Passagem de parâmetros:
-- Por valor (cópia)

        int i = 10;       //nome do método: "fazerAlgo"
        public void fazerAlgo(int i) {
        i = i + 10;
        System.out.println("Valor de i dentro: " + i); // -> Resultado = 20
        }
        System.out.println("Valor de i dentro: " + i); // -> Resultado = 10 pq o valor de i veio por cópia, de fora dos {}. 

-- Por referência (endereço) - Relacionada a orientação ao objeto. É o posto da passagem por valor. 

- Boas Práticas
-- Nomes devem ser descriticos, porém curtos; 
-- Notação camelo: 
        
        "verificarSaldo(); 
        executarTransferencia (...); 
        existeDebito();"

    -- Deve possuir entre 80 e 120 linhas; // Quanto mais linhas, mais dificil de entender. Recomenda-se criar outros métodos e organizar para que um chame o outro. 
    -- Evite lista de parâmetros longas.
    -- Visibilidades adequadas para criar métodos fáceis de entender.
    







