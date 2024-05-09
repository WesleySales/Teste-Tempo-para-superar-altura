
### Exércicio: 

Sabendo que João tem 1,20m de altura e cresce 0,02m por ano e que Charles tem 1,05m e cresce 0,03m por ano
faça um programa que informe quantos anos serão necessários para que Charles fique mais alto que João.

##

    #include <stdio.h>
    #include <locale.h>
    #include <string.h>

    int main (){
    	setlocale(LC_ALL,"Portuguese");
    	int contador=0;
    	double altura_joao=1.20, altura_charles=1.05;
    	
    	while (altura_joao>altura_charles)
    	{
    		altura_joao+=0.02;
    		altura_charles=altura_charles+0.03;
    		contador+=1;
    	}
    	printf("Para Charles passar a altura de Joao foram %d anos",contador);
    		
    
    }

Resolvido usando uma estrutura básica While, na qual os acréscimos de altura são feitos até que a condição "Altura_João>=Altura_Charles" seja falsa.
Acrescentei uma variável "contador=0" que vai somar 1 a cada vez que a condição for verdadeira e quando ela for finalmente quebrada retornará os anos.
