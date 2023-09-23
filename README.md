# Loop-for-no-java

Anotações do loop for no java

                                                                          Loop for
Agenda
.Controle for

                                                                         Comando for

.Executa um bloco de código que está dentro do comando for enquanto uma expressão for verdadeira.
.Muuuito utilizado na programação.

for (inicialização; condição; atualização) {
    //bloco de código
}

                                                                         for "normal"
for(int i = 0; i < 5; i++) {
   System.out.println("i tem valor: " + i);

Para esse comando existem algumas variações, a primeira variação desse comando séria o normal onde a gente inisializa um contador a gente adiciona uma
expressão booliana que seria o i menor que 5 e a gente atualiza a variavel do i que seria o i++ e dentro desse código do fórum a gente coloca alguma lógica
de programção que nesse caso seria impremir o valor de i vamos ver isso na prática.

EX1:

package com.madu.LoopFor;

public class LoopFor {

	public static void main(String[] args) {
		
		for (int i=0; i < 5 ; i++){
			System.out.println("i tem valor: " + i);
		}
		
		//System.out.println(i);
		
		for (int i=5; i > 0 ; i--){
			System.out.println("i tem valor: " + i);
		}
	}

}


Console:

i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4
i tem valor: 5
i tem valor: 4
i tem valor: 3
i tem valor: 2
i tem valor: 1

Ex2:

package com.madu.LoopFor;

public class LoopFor {

	public static void main(String[] args) {
		
		for (int i=0; i < 5 ; i++){
			System.out.println("i tem valor: " + i);
		}
	}

}


Console:
i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4

                                                                  for com mais de uma variável

for (int i = 0, j = 10; i < j; i++, j--) {
    System.out.println("i tem valor: " + i + "e j tem valor: " + j);


A gente também pode fazer o for com mais de uma variável, quando a gente usa mais uma variável nós separamos através de vírgula, o ponto e vírgula ele vai
separar a inicialização da expressão com a atualização quando a gente utiliza mais uma variável a gente separa por vírgula então aqui a gente pode fazer
mais um exemplo.

Ex1:

package com.madu.LoopFor;

public class LoopFor {

	public static void main(String[] args) {
		
		for (int i=0; i < 5 ; i++){
			System.out.println("i tem valor: " + i);
		}
		
		//System.out.println(i);
		
		for (int i=5; i < 0 ; i--){
			System.out.println("i tem valor: " + i);
		}
		
		for (int i=0, j=10 ; i < j ; i++, j--) {
			System.out.println("i = " + i + "; j = " + j);
		}
	}

}

Console:
i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4
i = 0; j = 10
i = 1; j = 9
i = 2; j = 8
i = 3; j = 7
i = 4; j = 6

                                                              partes ausentes

int i = 0;
for (; i < 5; ) {
    System.out.println("i tem valor: " + i);
    i++;
}

A gente também pode utilizar o for com partes ausentes isso aqui não é muito comum a maneira mais comum de a gente utilizar o for na programação é a
primeira forma que seria o for normal que tem o i=0 e i menor que algum valor e i++ que a gente tem a inicialização a expressão e a atualização
mas a gente também pode utilizar com partes ausentes, pode ser que o programa que você esteja fazendo requer que você faça isso então tudo bem você
pode utilizar.

Ex1:
package com.madu.LoopFor;

public class LoopFor {

	public static void main(String[] args) {
		
		for (int i=0; i < 5 ; i++){
			System.out.println("i tem valor: " + i);
		}
		
		//System.out.println(i);
		
		for (int i=5; i < 0 ; i--){
			System.out.println("i tem valor: " + i);
		}
		
		for (int i=0, j=10 ; i < j ; i++, j--) {
			System.out.println("i = " + i + "; j = " + j);
		}
		
		int count = 0;
		for ( ; count < 10 ; ) {
			System.out.println("valor de count: " + count);
			count += 2;
		}
	}

}

Console:
i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4
i = 0; j = 10
i = 1; j = 9
i = 2; j = 8
i = 3; j = 7
i = 4; j = 6
valor de count: 0
valor de count: 2
valor de count: 4
valor de count: 6
valor de count: 8

Ex2:

package com.madu.LoopFor;

public class LoopFor {

	public static void main(String[] args) {
		
		for (int i=0; i < 5 ; i++){
			System.out.println("i tem valor: " + i);
		}
		
		//System.out.println(i);
		
		for (int i=5; i < 0 ; i--){
			System.out.println("i tem valor: " + i);
		}
		
		for (int i=0, j=10 ; i < j ; i++, j--) {
			System.out.println("i = " + i + "; j = " + j);
		}
		
		int count = 0;
		for ( ; count < 10 ; ) {
			System.out.println("valor de count: " + count);
			count += 2;
		}
		
		for (int cont = 0; cont < 10; cont += 2) {
			System.out.println("valor de cont: " + cont);
		}
	}

}

Console:
i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4
i = 0; j = 10
i = 1; j = 9
i = 2; j = 8
i = 3; j = 7
i = 4; j = 6
valor de count: 0
valor de count: 2
valor de count: 4
valor de count: 6
valor de count: 8
valor de cont: 0
valor de cont: 2
valor de cont: 4
valor de cont: 6
valor de cont: 8

O ex1 e ex2 é a mesma forma mais caso seja preciso a gente pode utilizar com partes ausentes também.

                                                           loop infinito
for (;; );

Existe também o loop infinito que os eu programa nunca vai parar de rodar que seria o foco apenas os dois ponto e vírgula dentro dele, é a mesma coisa que um
while true e aí o bloco la´dentro vazio porém também tem o loop infinito, muito importante não tenetem isso em casa se não vocês vão ter que tirar a tomada
da parede para poder parar o programa se não o programa numca vai terminar de executar, e é melhor não tentar isso, mas isso é um a curiosidade.

                                                          loop sem corpo

int soma = 0;
for (i = 1; i < 5; soma += i++);
System.out.println("O valor da soma é: " + soma);

Também tem o loop sem corpo, isso aqui seria mais utilizado para quando você quer somar valores.

Ex:
package com.madu.LoopFor;

public class LoopFor {

	public static void main(String[] args) {
		
		for (int i=0; i < 5 ; i++){
			System.out.println("i tem valor: " + i);
		}
		
		//System.out.println(i);
		
		for (int i=5; i < 0 ; i--){
			System.out.println("i tem valor: " + i);
		}
		
		for (int i=0, j=10 ; i < j ; i++, j--) {
			System.out.println("i = " + i + "; j = " + j);
		}
		
		int count = 0;
		for ( ; count < 10 ; ) {
			System.out.println("valor de count: " + count);
			count += 2;
		}
		
		for (int cont = 0; cont < 10; cont += 2) {
			System.out.println("valor de cont: " + cont);
		}
		
		int soma = 0;
		for (int i=0; i < 5; soma += i++);
		System.out.println("O valor da soma é: " + soma);
	}

}

Console:
i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4
i = 0; j = 10
i = 1; j = 9
i = 2; j = 8
i = 3; j = 7
i = 4; j = 6
valor de count: 0
valor de count: 2
valor de count: 4
valor de count: 6
valor de count: 8
valor de cont: 0
valor de cont: 2
valor de cont: 4
valor de cont: 6
valor de cont: 8
O valor da soma é: 10

Sem chaves nos blocos.

Ex2:
	  
		int soma = 0;
		for (int i=0; i < 5; soma += i++);
		System.out.println("O valor da soma é: " + soma);
		
		for (int i=0; i < 5 ; i++)
			System.out.println("i tem valor: " + i);
	  }
	}



Console:
O valor da soma é: 10
i tem valor: 0
i tem valor: 1
i tem valor: 2
i tem valor: 3
i tem valor: 4

Isso não é muito recomendavé, por que só a primeira linha do for vai ser executada.

                                                                   loop melhorado

.Muito utilizado com Arrays

Existe também um ouro loop melhorado, ele na verdade foi foi introduzido no java 5 ele é muito utilizado com arrays quando a gente estudar arrays a gente
volta para a questaõ dos loops melhorados, ele eé amplamente utilizado é muito utilizado na programação.
