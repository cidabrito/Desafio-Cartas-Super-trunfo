# Desafio-Cartas-Super-trunfo 
criei o printf

#include<stdio.h>

int main(){
    printf("Desafio Super trunfo- cadastro de cidades!\n");

    int codigo;
    char nome[50];
    int populacao;
    float area;
    float pib;
    int pontos_turisticos;
    printf("\nDigite o codigo da cidade: ");
    scanf("%d", &codigo);

    printf("Digite o nome da cidade: ");
    scanf("%[^\n]", nome);

    printf("Digite a populacao (em milhoes): ");
    scanf("%d", &populacao);

    printf("Digite a area da cidade (em km): ");
    scanf("%f", &area);

    printf("Digite o pib da cidade (em bilhoes de dólares): ");
    scanf("%f", &pib);

    printf("números de ponto turísticos: ");
    scanf("%d", &pontos_turisticos);


    printf("\nDados da cidade cadastrada\n");
    printf("Codigo: %d\n", codigo);
    printf("Nome: %s\n", nome);
    printf("Populacao: %d milhoes\n", populacao);
    printf("Area: %.2f km", area);
    printf("Pib: %.2f bilhoes de dólares\n, pib");
    printf("Pontos turisticos: %d\n", pontos_turisticos);
    return 0;


}
