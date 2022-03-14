# jadienne-logica02]
(1)Questão

#include <stdio.h>


int soma(int valor) {
if(valor == 0) {
      return 0;
    } else {
return valor + soma(valor -1);
}
}

int main(){
int num=0, i=0, r=0;

printf("Digite o numero\n");
scanf("%d", &num);

r=soma(num);
printf("Valor somado %d\n", r);
}



(2)QUestão

#include <stdio.h>
#include <locale.h>

float segundos(float H, float M, float S) {
float min,calculo,ho;
calculo=(S+(M*60)+(H*60*60));

return calculo;

}

int main () {

setlocale(LC_ALL, "Portuguese");

float H,M,S;

printf("\nDigite a hora, o(s) minuto(s) e o(s) segundo(s): \n");

scanf("%f%f%f",&H,&M,&S);

printf("\nO total de segundos são: %f",segundos(H,M,S));

}


  (3) Questão
  
  #include <conio.h>
#include <math.h>

#define PI 3.14

float Volume(float raio) {
    float v=4/3*(PI*pow(raio,3));
    return v;
}

int main() {
    float Raio, Resultado;

    printf("Digite o raio de uma esfera para calcular o volume:\n");
    scanf("%f", &Raio);

    Resultado=Volume(Raio);
    printf("%.3f\n", Resultado);

    getchar();
    return 0;

}


  (5) questão
  
#include <stdio.h>

int main() {
int numero;
    printf ("Digite um numero\n");
    scanf("%d", &numero);
 if(numero >=0) {
    printf("%d e um numero positivo.\n ", numero);
        return 1;
    } else {
      printf("%d e um numero negativo.\n ", numero);
        return 0;
    }
            return 0;
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


(8) Questão


#include <stdio.h>

int main()
{
    int fat, n;
    printf("Insira um valor para calcular o fatorial:\n ");
    scanf("%d", &n);

    for(fat = 1; n > 1; n = n - 1)
        fat = fat * n;

    printf("\nFatorial calculado: %d", fat);
    return 0;
}
