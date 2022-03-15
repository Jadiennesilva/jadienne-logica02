# jadienne-logica02]

(1) Questão 

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

(2) Questão 

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

(3) Questão 

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

(4) Questão 

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

(5)

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

(6) Questão

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


(7) Questão

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


