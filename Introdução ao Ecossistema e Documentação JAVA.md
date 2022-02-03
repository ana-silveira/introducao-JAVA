 02 e 03/02/2022
1) Intrudução ao ecossistema JAVA:
 
* Apresentação do curso - OK
     
* Introdução ao ecossistema JAVA
   -  Linguagem de programação e plataforma computacional lançada em 1995 pela Sum Microsystems
   - Caracteristicas: Linguagem Compilada, linguagem interpretada, fortemente tipada, de alto nível (toda a programação é orientada a objetos)
   - Executada em uma máquina virtual (JVM)
   - Como funciona? O código fonte .java é compilado/interpretado pelo JAVA compiler (JAVAC) para um executável chamado Bytecodes, de extensão .class,  onde esses bytecodes são interpretados pela JVM.      
* Entendendo a JVM
   - É uma máquina virtual resp. pela tradução dos bytecodes oriundos do compilador javac, em código de máquina de cada sistema operacional. 
   - Caracteristicas: Responsável pela execução das pilhas, pelo gerenciamento de memória, gerenciamento e execução de threads, otimização de código (contém uma feature de compilação JIT - Just in Time) e Garbage Collector (GC - limpeza de memória)
   - Diferença do JAVA para as outras linguagens compiladas: 
   -- O JAVA compila todo o código fonte usando o javac por um executável bytecode, e o bytecode já faz a tradução do código para cada sistema operacional (WIN, LIN ou MAC). Já outras linguagens compiladas precisam que seu código fonte seja escrito especificamente para cada sistema operacional, pois não existe essa etapa de tradução conforme o SO. 
    - Quais as diferenças entre JRE e JDK?
    -- JRE (Java Runtime Environment) - Responsável por executar os programas em JAVA.
    -- JDK (Java Development Kit) - Utilitários que permitem o desenvolvimento de programas em JAVA; Já possuem a JVM para executar os programas. 
    - Tipos de plataformas JAVA: SE (Standard Ed.) x EE (Enterprise Ed.) x ME (Micro Ed.)
    - Implementações do JAVA SE: Focaremos na OpenJDK

*Instalando a JVM
    - (Segui a instalação do prof. Nelio Alves, do curso da Udemy => https://www.youtube.com/watch?v=QekeJBShCy4)

* Executando um programa JAVA


-------------------------