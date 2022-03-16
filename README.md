# jadienne-logica02]

(1) Respostas 

#include <stdio.h>

//CabeÃ§alho da funÃ§Ã£o 
void sNumeros(float);

int main () {
       
    float n;
    printf ("Digite um nÃºmero\n");
    scanf("%f",&n);
    
    //funÃ§Ã£o sendo chamada
    sNumeros(n);
    
return 0;
};

// Corpo da funÃ§Ã£o
void sNumeros(float n) {
    //Para resolver esse problema usaremos a formula da soma de Gauss que Ã© "Sn = ((a1 + an) * n) /n "
    
   float t; // t Ã© o valor total da soma dos nÃºmeros
   
   float  i = 1;  // i Ã© o nÃºmero inicial, ou seja o menor nÃºmero.
   
    t = ((i + n)*n)/2 ;
    printf("%g",t);
};

(2) Respostas 

#include <stdio.h>
void tParaS (float, float, float);

 void tParaS (float H, float M, float S)  {
 
  float sCalculoH, sCalculoM, ho;
	sCalculoH = 3600 * H;
	sCalculoM = 60 * M;
	ho = sCalculoH + sCalculoM + S;
}

int main () {
	
	float H,M,S;
	
	printf("\n Digite a hora");
	scanf("%f",&H);
	
	printf("\n Digite os minutos");
	scanf("%f",&M);
	
	printf("\n Digite os segundoa");
	scanf("%f",&S);
	
	//printf("%g",tParaS(H, M, S));	
	tParaS(H, M, S);
	
	return 0;
}

(3) Respostas 

#include <stdio.h>

float divisao(int, int);


int main () {
	
	int a, b;
	
	printf("Digite um numero");
	scanf("%d",&a);
	
	printf("Digite o segundo numero");
	scanf("%d",&b);
	
	divisao(a, b);

	printf("%g",divisao(a,b));
	return 0;
}


float divisao (int a, int b) {
	
	if (a % b == 0) {
		    
	return 0;
	
	} else if  (a % b != 0 & a < b){
	do {
				
	b = --b;
	 
	return b;
	
	}while (a % b != 0);
	
} else {
	
	do {
		
	b = ++b;
					
return b;
			
} while (a % b != 0 );

	}
		
}

(4) Respostas 

#include<stdio.h>
#include<math.h>
int main()
{

float raio (float);

float v, ra;

printf ("Digite o raio de uma esfera");
scanf("%f",&ra);

raio(ra);

printf("%f",raio(ra));
return 0;
}

float raio (float ra) {

float v, r;
r = pow(ra,3);
v = 4.0/3.0 * r;

return v;
}

(5)Respostas 

#include<stdio.h>


void vefify (int);

int main() {   
int n;

    printf("Vericar se o numero Ã© positivo\n");
    printf("Digite um numero");
    
    scanf("%d",&n);
    
    verify(n);
    
    return 0;
}

void verify (int n) {
 
if (n > 0) {

printf ("O nÃºmero Ã© positivo ");

} else {
 printf ("O nÃºmero nÃ£o Ã©positivo");
}

}

(6) Respostas 

 #include <stdio.h> 
 #include <stdlib.h> 
 #include <locale.h> 
  
 float pesoideal(float altura, char sexo); 
  
 int main() { 
   setlocale(LC_ALL, "Portuguese_Brazil"); 
    
   float A; 
   char S; 
    
  printf("Digite o seu sexo; M ou F: "); 
  scanf("%c", &S); 
    
   printf("Digite a sua altura: "); 
   scanf("%f", &A); 
    
   pesoideal(A, S); 
    
    
 } 
  
 float pesoideal(float altura, char sexo) { 
   float peso; 
    
   if(sexo == 'M') { 
     peso = 72.7 * altura - 58; 
     printf("\nO seu peso ideal é: %2.2f kg", peso); 
   } else if(sexo == 'F') { 
     peso = 62.1 * altura - 44.7; 
     printf("\nO seu peso ideal é: %2.2f kg", peso); 
   } 
    
   return peso; 
 }
 
(7) Respostas 

#include <stdio.h>
#include <conio.h>
float calc_media()
{
    float soma, num, media, i;

    soma = 0;
    i = 0;
    num = 1;

    while(num != 0)
    {
        printf("\nDigite um numero positivo\n");
        scanf("%f", &num);

        while(num < 0)
        {
            printf("\nNumero invalidao!");
            printf("\nDigite um numero positivo novamente");
            scanf("%f", &num);
        }

        soma += num;

        i++;
    }

    media = soma/(i-1);

    return media;
}
int main()
{
    float r;

    r = calc_media();

    printf("O valor da media aritmetica foi %.2f",r);

    getchar();
}


(9) respostas

#include <stdio.h> 
 #include <stdlib.h> 
 #include <locale.h> 
  
 int soma(int n); 
  
 int main() { 
   setlocale(LC_ALL, "Portuguese_Brazil"); 
    
   int numero, resultado; 
    
   printf("Digite um número inteiro e positivo: "); 
   scanf("%d", &numero); 
    
   resultado = soma(numero); 
    
   printf("\nA soma dos divisores do número é: %d", resultado); 
 } 
  
 int soma(int n) { 
   int divisores, soma = 0;  
    
   for(divisores = 1; divisores <= n; divisores++) { 
     if(n % divisores == 0) { 
       soma = soma + divisores;  
     } 
   } 
    
   return soma; 
 }


(24) Respostas


#include <stdio.h>
#include <stdlib.h>

int main() {
    int i, indiceMaior, indiceMenor;
    float menor = 99, maior = 0, temp[12];

    for(i = 0; i < 12; i++) {
        printf("Digite a temperatura do mes %d: ", i + 1);
        scanf("%f", &temp[i]);
    }

    for(i = 0; i < 12; i++) {
        if(menor > temp[i]) {
            menor = temp[i];
            indiceMenor = i;
        }
        if(maior < temp[i]) {
            maior = temp[i];
            indiceMaior = i;
        }
    }

    printf("A menor temperatura foi %.2f e ocorreu no mes ", menor);
    switch(indiceMenor) {
    case 0:
        printf("Janeiro\n");
        break;
    case 1:
        printf("Fevereiro\n");
        break;
    case 2:
        printf("Marco\n");
        break;
    case 3:
        printf("Abril\n");
        break;
    case 4:
        printf("Maio\n");
        break;
    case 5:
        printf("Junho\n");
        break;
    case 6:
        printf("Julho\n");
        break;
    case 7:
        printf("Agosto\n");
        break;
    case 8:
        printf("Setembro\n");
        break;
    case 9:
        printf("Outubro\n");
        break;
    case 10:
        printf("Novembro\n");
        break;
    case 11:
        printf("Dezembro\n");
        break;
    }

    printf("A maior temperatura foi %.2f e ocorreu no mes ", maior);
    switch(indiceMaior) {
    case 0:
        printf("Janeiro\n");
        break;
    case 1:
        printf("Fevereiro\n");
        break;
    case 2:
        printf("Marco\n");
        break;
    case 3:
        printf("Abril\n");
        break;
    case 4:
        printf("Maio\n");
        break;
    case 5:
        printf("Junho\n");
        break;
    case 6:
        printf("Julho\n");
        break;
    case 7:
        printf("Agosto\n");
        break;
    case 8:
        printf("Setembro\n");
        break;
    case 9:
        printf("Outubro\n");
        break;
    case 10:
        printf("Novembro\n");
        break;
    case 11:
        printf("Dezembro\n");
        break;
    }

    return 0;
}

