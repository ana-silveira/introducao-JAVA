Programação Orientada a Objetos

Introdução

Objetivos: Possibilitar que o aluno compreenda todos os conceitos relativos a programação orientada a objetos. 

Por que devemos programar orientado a objetos?
PE (paradigma estruturado) vs POO :
    -- PE tem uma representação mais simplista, limitada de se programar, é de mais baixo nível. já o POO é mais representativo do mundo real, possuindo mecanismos mais avançados se comparados a PE.  
    -- PE foca em operações (funções) e dados . POO facilita e foca na modelagem de entidades e nas interações entre estas (é de mais alto nível, mais avançada, de maior quantidade). --> Nível de abstração maior do que em linguagens estruturadas. 
    -- PE foca mais no "como fazer"; POO foca mais no "o que fazer" (qual o problema a ser resolvido e não o "como resolver o problema"). Isso facilita a atividade de programação, contribuindo com a automatização de processos mais rapidamente. 
    
Vantagens da POO:
-- Melhor coesão (as ideias estão trabalhando em conjunto, dizendo respeito as mesmas coisas. Responsabilidades bem definidas);
-- Melhor acoplamento (bons acoplamentos são flexiveis. PEs tem acoplamentos mais rígidos).
-- Diminuição de GAP semântico.  (diminuição da diferença de representação entre o mundo real e o semântico ao comparar PE e POO. Os dois mundos ficam mais próximos)
-- Coletor de lixo (a medida que vamos programando, o software trabalha, a memória vai sendo ocupada. Existem mecanismos na POO que vão limpando essa memória na medida que objetos não vão mais sendo utilizado, e liberando-a para, por ex., o computador não travar. PE não possuem esses mecanismos; O programador precisa se preocupar com liberação de memória do computador para fazer a linguagem funcionar, e isso é muito "baixo nível".  )

RESUMO: PE foca em dados brutos e funções/procedimentos para manipulação desses dados. Já na POO existem objetos que representam entidades do mundo real, e elas se relacionam entre si para resolver o problema. Pensa-se mais nas estruturas que serão utilizadas e não nos conceitos e ideias que serão manipulados. Isso faz diferença na capacidade de resolver os problemas da melhor forma possivel. 

Estrutura básica da OO (Orientação a Objetos)
-- O que é OO? É um paradigma de análise, projeto e programação de sistema de software, baseado na composição e interação entre diversas unidades de software chamadas objetos. 
-- Fundamentos: 
1. **Abstração**: Processo pelo qual se isolam características de um objeto, considerando os que tenham em comum certos grupos de objetos. É a capacidade de pensar nas caracteristicas essenciais e deixar de lado as acidentais; Assim é possivel ter maior reuso dessas entidades e sendo possivel usá-la em varios pontos diferentes da aplicação. Abstração é pensar no que é essencial e no reuso. 
2. **Reuso**: Capacidade de criar novas unidades de código a partir de outras já existentes. Esse mecanismos em linguagens não orientadas é mais arcaico, mais baixo nível. Nas orientadas existe mais diversidade de mecanismos e formas de reuso. 
3. **Encapsulamento**: É a capacidade de esconder complexidades e proteger dados. (Criação de camadas de proteção para impedir acessos indevidos. Isso é mais fácil para POO do que PE)

-----------------
Aula 3> Apresentação dos conceitos que criam as estruturas básicas da OO: Classe, Atributo, Método, Objeto e Mensagem. 
1. Classes: É uma estrutura que abstrai um conjunto de objetos com caracteristicas similares. Uma classe define o comportamento de seus objetos através de métodos e os estados possíveis destes objetos através de atributos. Em outros termos, uma classe descreve os serviços providos por seus objetos e quais informações eles podem armazenar. ===> Classe é a base de tudo!!! Ela serve de molde para modelar o conceito do mundo real. 
-- Dicas: Nomes contendo substantivos; nomes significativos; considerar o contexto! Ex: Pessoa x Aluno, professor, vendedor etc
-- Código: 

            class Carro { 
            }

2. Atributo: É o elemento de uma classe responsável por definir sua estrutura de dados. O conjunto destes atributos será responsável por representar suas características e fará parte dos objetos criados a partir da classe. Os atributos caracterizam as nossas classes!
-- Atributos x Variáveis > A: "O que é próprio e peculiar a alguém ou a alguma coisa"; ** Criamos dentro das classes** . V: "Sujeito a variações ou mudanças; que pode variar; inconstante, instável."" **Variáveis nós criamos dentro dos métodos**. 
-- Dicas: Substantivos e adjetivos ("carro branco"); nomes significativos; considerar o contexto para defninir adequadamente os atributos da classe; abstração; tipos adequados de dados. 
-- Código: 

        class Carro {
            int portas;
            String cor;
            String modelo;
            int capacidadeTanque;
        }

3. Método: É uma porção de código (sub-rotina) que é disponibilizada pela classe. Este é executado quando é feita uma requisição a ele. Um método serve para identificar quais serviços ou **ações** a classe oferece. Métodos são responsáveis por definir e realizar um determinado comportamento. 
-- Criação do método: Visibilidade, retorno (atrelado ao tipo de dado), nome (do método), parâmetros (caso precise).
-- Dicas: Verbos; nomes significativos; contexto deve ser considerado. 

        class Carro {
           void frear (){
           ...
               }
        }

- Dois métodos especiais:
    -- Construtor: Constrói/cria objetos. Cada linguagem tem uma forma de definir um construtor. Em java, é obrigatório que o nome da classe seja igual ao nome do construtor. Ele não precisa estar explicito, e ainda assim poderá ser chamado. O VOID não é obrigatório. 

        class Carro {
           Carro (){
           ...
               }
        }
        
    -- Destrutor: Auxilia na criação do objeto. Ex: Coletor de lixo chama o destrutor antes de apagar os dados/classes/objetos não utilizados. Diferente do Construtor, o VOID é obrigatório de ter. 
    
        class Carro {
           void finalize (){
           ...
               }
        }

    -- Sobrecarga: Mudar a assinatura de acordo com a necessidade. Obs: Assinatura = nome + parâmetros. (Obs: Não existe sobrecarga em Python.)
    
      m1 ()
      m1 (int i)
      m1 (float f)
      m1 (String s, long l)
      m1 (long l), String s)
    
- Exercitando:

        class Carro {
            int portas;
            String cor;
            String modelo;
            int capacidadeTanque;
  
            // Construtor
            
            Carro() {
                }
            
            //Sobrecarga
             Carro(String cor, Atring modelo, int capacidadeTanque) {
                this.cor = cor;
                this.modelo = modelo;
                this.capacidadeTanque = capacidadeTanque;
            }
            
            
            void setCar(String cor) {
                this.cor = cor;
                }
            
             String getCar() {
                return cor;     // como retorna a cor, não pode ser void. 
                }
            
            void setCapacidadeTanque(int capacidadeTanque){
                this.capacidadeTanque = capacidadeTanque;
            }
            
            getCapacidadeTanque (){
                return capacidadeTanque;
            }
        
        //     Método do total para encher o tanque:
        
            double totalValorTanque (double valorCombustivel) {
                return capacidadeTanque * valorCombustivel;
            }
        }
        
=> Uma boa prática: Inserir o construtor logo após a declaração dos tipos de dados das variáveis, seguido dos gets e sets, e métodos de negócio por último caso existam. 

4. Objeto: Um objeto é a representação de um conceito/entidade do mundo real, que pode ser física (bola, carro, árvore etc) ou conceitual (viagem, estoque, compra etc) e possui um significado bem definido para determinado software. Para esse conceito/entidade, deve ser definida inicialmente uma classe a partir da qual posteriormente serão instanciados objetos distintos.
- Qual a diferença entre classe e objeto? A classe é estática, um molde; e é definida para dizer o que vai manipular os nossos objetos, ou seja, o que executa de fato são os objetos. Para fazer com que a classe funcione, é necessário criar objetos a partir dela. Eles é que irão funcionar. Objetos são instâncias de classes.
- Criação: 

        Carro carro = new Carro ();  // 
        TipoDaVariavel Atributo/variável = operadorNew  construtor(); construtor() o objeto. Parenteses vazio = default. 

5. Mensagem: É o processo de ativação de um método de um objeto. Isto ocorre quando uma requisição (chamada) a esse método é realizada, assim disparando a execução de seu comportamento descrito por sua classe. Pode também ser direcionada diretamente à classe, caso a requisição seja a um metodo estático. 

        Carro carro = new Carro();     (criação do objeto)
        carro.<método>;             (mensagem para a chamada do objeto)
        
        Carro.<método>;   (mensagem para a chamada da classe - obs: C maiúsculo diferencia a classe!)
        
Obs> Conceitos mais avançados de OO que não serão explorados neste curso. 
a) Instância x Estático: atributos e métodos;
b) Estado de um objeto; ()
c) Identidade de um objeto;
c) Representação numérica de um objeto;
d) Representação padrão de um objeto. 


As relações: Herança, associação e interface

Objetivos: Apresentar os conceitos que ajudam a criar entidades a partir de outras entidades. 
- Herança;
- Associação;
- Interface.


1. Herança: É o relacionamento entre classes em que uma classe chamada subclasse (classe filha, classe derivada) é uma extesão, um subtipo, de outra classe chamada de superclasse (classe pai, classe mãe, classe base). Devido a isso, a subclasse consegue reaproveitar atribuots e metodos dela. Além dos que venham a ser herdados, a subclasse pode definir seus próprios membros (atributos e métodos).

    **A finalidade da herança é criar subtipos, e não para reuso!** Reuso pode ser uma consequência da sua finalidade. É possivel ter reuso sem herança. 
    
           // A está herdando atributos e métodos de B
           class A extends B {        
                ...
            }
    
    Tipos de Herança:
       -- Simples: A classe filha só tem uma classe mãe. 
       -- Multipla: A classe filha tem mais de uma classe mãe. JAVA NÃO TEM HERANÇA MULTIPLA (Python e C# tem)!
       
    Herança -  Upcast e Downcast:
        -- Upcast: classes filhas --> classe mãe (os tipos sobem na hierarquia de classes; sobe para uma classe mais genérica). 
        
            A a = new B(); // estou transformando B em A. Está implicito a herança upcast na escrita do Java.
            
       -- Downcast: classe mãe --> classes filhas (os tipos de classe descem na hierarquia de classes, ocorre um aprofundamento da hierarquia)
       
        B a = (B) new A (); // Aqui é explicito; eu tenho que dizer pra quem em quero transformar. Pego new A() e transformo na variável do tipo B. É comum ocorrencia de erros na compilação de downcast e não é recomendável na maioria dos casos. 
        
    Herança - Polimorfismo:
        - A mesma ação, se comprotando diferente. ==> A possibilidade de um mesmo método de se comportar diferente. . Traz grande flexibilidade ao código!!! Obs: Nem toda herança tem polimorfismo. 
        
    Herança - Sobrescrita:
        - A mesma ação, **podendo** se comportar diferente. 

2. Associação: Possibilita um relacionamento entre classes/objetos, no qual estes possam pedir ajuda a outras classes/objetos e representar de forma completa o conceito ao qual se destinam. Neste tipo de relacionamento, as classes e os objetos interagem entre si para atingir seus objetivos. 
Aqui, diferente da Herança, não existem subtipos, mas sim um usa o outro.

    2 tipos:
- Estrutural: 
    -- Composição: "Com parte todo". Grande relação de dependência e existência entre as partes. Um é composto pelo outro e o 1o depende do 2o para existir. 

        class Pessoa {
        Endereco endereço;
        }
        // Se a pessoa deixar de existir, o endereço perde o sentido porque esse endereço é o da pessoa. --- Pensar no mundo real!
    
    -- Agregação: "Sem parte todo". Uma parte pode existir sem o todo. 
    
        class Disciplina {
        Aluno aluno;
        }
        // Se a disciplina deixar de existir, o aluno não necessariamente vai deixar de existir porque podem existir, por exemplo, outras disciplinas.  
    
- Comportamental:
    -- Dependência: "Depende de".  

        class Compra {
        ...
        finalizar (Cupom cupom, ...);
        ...
        }    

Resumo:
Herança (+ rigida a relação entre as partes; **uma coisa é a outra?** É subtipo da outra? uso HERANÇA) 
x
Associação (relação mais flexivel; **Uma coisa não é a outra**, mas uma vai usar a outra; então faço ASSOCIAÇÃO): 


3. Interface: Define um contrato que deve ser seguido pela classe que a implementa. Quando uma classe implementa uma interface, ela se compromete a realizar todos os comportamentos que a interface (Windows, Mac, Linux, Ubuntu etc) disponibiliza.

        interface A {
            ...
         }
         class B implements A {
            ...
         }

Conceitos avançados importantes:
-- Tipos de classe: Abstrata e Concreta
-- Métodos abstratos
-- Características das associações
-- Palavras coringas: super (Java), base (C#), super() (Python);
-- Relações entre classes e interface: extends e implements

A organização dos pacotes e visibilidades

Objetivos: Apresentar os conceitos que organizam a OO:
1) Pacotes: 
- São uma organização física (pastas e subpastas contendo arquivos, dentro do sistema operacional)  ou lógica (dentro do mesmo pacote há uma separação lógica dos arquivos, pacotes virtuais) criada para separar classes com responsabilidades distintas. Com isso, espera-se que a aplicação fique mais organizada e seja possivel separar classes de finalidades e representatividades diferentes. 
- São criados da seguinte forma: 

        package ...; (Separa e cria classes )
        import ...; (Torna visivel as classes que eu vou precisar; Dentro de uma classe eu preciso importar outra classe que está em outro pacote )
    

2) Visibilidades (modificadores de acesso): Determinam até que ponto uma classe, atributo ou método pode ser usado. A utilização de modificadores de acesso é fundamental para o uso efetivo da OO. Algumas boas práticas e conceitos só são atingidos com o uso correto desses modificadores. 
- Tipos de visibilidades providas pela OO: 
    -- Private: Só será visivel dentro da classe. 
        
        private int i;
        private void do ();

    -- Protected: Visibilidade dentro da classe, mesmo pacote e subclasses. 

        protected int i;
        protected void do ();
        
    -- Public: Em qualquer lugar (sem restrições de visibilidade).
    
        public int i;
        public void do ();

- Qual usar?
-- Cada tipo tem uma finalidade; Deve-se avaliar dados(atributos/metodos)  que precisem de proteção, mas considerando que outros métodos de outras classes possam precisar de tais dados. 

Próximos passos
- Padrões de projeto (Design Patterns)
- Boas práticas: SOLID, código, técnicas de programação, etc
- Refatoração de código e como fazer
- UML (Linguagem de modelagem que não é unicamente utilizada para o OO, mas ficou mt conhecida para esse fim)
- Frameworks (softwares de alta qualidade hoje em dia são criados com frameworks pq ganham tempo e melhoram a qualidade, maiores e melhores resultados)
- Prática e estudo!




