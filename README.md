#include <stdio.h>

#define SUPER_TRUNFO.C
100

int main() {
    int codigos[MAX_CIDADES];
    char nomes[cidade simplesS][100];
    int populacoes[MAX_CIDADES];
    float areas[MAX_CIDADES];
    float pibs[MAX_CIDADES];
    int pontos_turisticos[MAX_CIDADES];

    int total, i;

    printf("Quantas cidades deseja cadastrar? ");
    scanf("%d", &total);

    for (i = 0; i < total; i++) {
        printf("\n--- Cadastro da cidade %d ---\n", i + 1);

        printf("Digite o codigo da cidade: ");
        scanf("%d", &codigos[i]);

        printf("Digite o nome da cidade: ");
        getchar(); // limpa o \n pendente
        scanf("%[^\n]", nomes[i]);

        printf("Digite a populacao (em milhoes): ");
        scanf("%d", &populacoes[i]);

        printf("Digite a area da cidade (em km²): ");
        scanf("%f", &areas[i]);

        printf("Digite o PIB da cidade (em bilhoes de dólares): ");
        scanf("%f", &pibs[i]);

        printf("Numero de pontos turisticos: ");
        scanf("%d", &pontos_turisticos[i]);
    }

    // Mostra os dados
    printf("\n\n===== Dados das Cidades Cadastradas =====\n");
    for (i = 0; i < total; i++) {
        printf("\nCidade %d\n", i + 1);
        printf("Codigo: %d\n", codigos[i]);
        printf("Nome: %s\n", nomes[i]);
        printf("Populacao: %d milhoes\n", populacoes[i]);
        printf("Area: %.2f km²\n", areas[i]);
        printf("PIB: %.2f bilhoes de dólares\n", pibs[i]);
        printf("Pontos turisticos: %d\n", pontos_turisticos[i]);
    }

    return 0;
}
   
