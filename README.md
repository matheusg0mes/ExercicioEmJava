# ExercicioEmJava
Aprendendo uma nova linguagem, dessa vez o Java, aqui vou deixar alguns exercício realizados para fixação da linguagem

import java.util.Locale;
import java.util.Scanner;

public class Main { 

	public static void main(String[] args) {
 //-----------------------------------------------------------------------------------
  //Exercicio para calcular quanto um funcionario ganha por mes--------------------------------------------------------------
  
  	Locale.setDefault(Locale.US);
	Scanner  sc = new Scanner(System.in);
 
int Func, Horas;
double Ganho, resultado;

System.out.printf("Digite o numero de funcionarios");
Func = sc.nextInt();
System.out.println("Digite o numero de horas");
Horas = sc.nextInt();
System.out.print("Quanto ganha por hora");
Ganho = sc.nextDouble();
resultado = Horas * Ganho;
System.out.printf("Number = %d %n SALARY + U$ %.2f",Func,resultado);  

	sc.close();

 //---------------------------------------------------------------------
 //Exercicio para calcular o valor total da compra de 2 produtos-------------------------------------------------
 
		Locale.setDefault(Locale.US);
	Scanner  sc = new Scanner(System.in);

	int code1, uni1, code2,uni2;
	double preco1,preco2, valor;
	
	System.out.println("Digite o codigo do produto");
	code1 = sc.nextInt();
	System.out.println("Digite a quantidade do produto");
	uni1 = sc.nextInt();
	System.out.println("Digite o preço do produto");
	preco1 = sc.nextDouble();
	
	System.out.println("Digite o codigo do produto");
	code2 = sc.nextInt();
	System.out.println("Digite a quantidade do produto");
	uni2 = sc.nextInt();
	System.out.println("Digite o preço do produto");
	preco2 = sc.nextDouble();
	
	valor = (preco1 * uni1) + (preco2 * uni2);
	
	System.out.printf("O valor a pagar : %.2f", valor);
	
	
	sc.close();
 
 //-----------------------------------------------------------------
 //Exercicio para calcular a area do triangulo,circulo,trapezio,quadrado e retangulo-----------------------------------------
 	Locale.setDefault(Locale.US);
	Scanner  sc = new Scanner(System.in);

	double A,B,C,Atriangulo, Atrapezio,Acirculo,Aquadrado,Aretangulo;
	double pi = 3.141159;
	
	System.out.println("digite o valor de A");
	A = sc.nextDouble();
	System.out.println("Digite o valor de B");
	B = sc.nextDouble();
	System.out.println("Digite o valor de C");
	C = sc.nextDouble();
	Atriangulo= A * C / 2;
	Acirculo= pi *(C* C);
	Atrapezio=(A + B) * C / 2;
	Aquadrado= B * B;
	Aretangulo=A * B;
	System.out.printf("TRIANGULO= %.3f%n CIRCULO= %.3f%n TRAPEZIO= %.3f%n QUADRADO= %.3f%n RETANGULO= %.3f%n",Atriangulo,Acirculo,Atrapezio,Aquadrado,Aretangulo);
	
	
	sc.close();
	}
	

}
 
