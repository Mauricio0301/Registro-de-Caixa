#include <stdio.h>
#include <stdlib.h>
#include <locale.h>
int main()
{
setlocale ( LC_ALL, "portugues");
int qtd, op;
float totalCompra = 0.0;
do
{
//Limpa Tela
system ("cls");
printf ("Codigo do Produto Comprado:");
printf ("\n\n");
printf ("Cachorro Quente\t|\tPreco:R$ 5.50\t|\tCodigo: 10\n");
printf ("Bauro Simples\t|\tPreco:R$ 4.00\t|\tCodigo: 20\n"); 
printf ("Sanduiche\t|\tPreco:R$ 3.50\t\|\tCodigo: 30\n"); 
printf ("Hamburguer\t|\tPreco:R$ 8.00\t\|\tCodigo: 40\n"); 
printf ("Refrigerante\t|\tPreco:R$ 3.00\t\|\tCodigo: 50\n");
printf ("\n\n");
printf ("[0] Para Finalizar a Compra\n");
scanf ("%d", &op);
//Limpa Tela
system ("cls");
switch(op)
{
case 10: printf("Cachorro quente. \n Digite a quantidade:");
scanf ("%d", &qtd);
totalCompra += qtd * 5.50;
printf ("Valor da compra: %.2f", totalCompra);
break;
case 20: printf("Bauro simples. \n Digite a quantidade:");
scanf ("%d", &qtd);
totalCompra += qtd * 4.00;
printf ("Valor da compra: %.2f", totalCompra);
break;
case 30: printf("Sanduiche. \n Digite a quantidade:");
scanf ("%d", &qtd);
totalCompra += qtd * 3.50;
printf ("Valor da compra: %.2f", totalCompra);
break;
case 40: printf("Hamburguer. \n Digite a quantidade:");
scanf ("%d", &qtd);
totalCompra += qtd * 8.00;
printf ("Valor da compra: %.2f", totalCompra);
break;
case 50: printf("Refrigerante. \n Digite a quantidade:");
scanf ("%d", &qtd);
totalCompra += qtd * 3.00;
printf ("Valor da compra: %.2f", totalCompra);
break;
case 0: printf ("Obrigado pela Compra, Volte sempre! \n");
break;
default: printf ("Opcao Invalida\n");
break;
}
} while(op != 0);
printf("Total da sua Compra e : %.2f", totalCompra);
return 0;
}
