#include <stdio.h>
int main() {
    
    char estado1[10];
    char codigo1[10];
    int populacao1;
    float area1;
    float pib1;
    int pontosturisticos1;

    char estado2[10];
    char codigo2[10];
    int populacao2;
    float area2;
    float pib2;
    int pontosturisticos2;

    float densidade_populacional1;
    float PIB_per_capita1;

    float densidade_populacional2;
    float PIB_per_capita2;

    float super_poder1;
    float super_poder2;
//variaveis
    printf("Bem vindo ao Super Trunfo! \n");
    printf("carta 1\n");

    printf("Digite o Estado:\n");
    scanf("%s", estado1);

    printf("Digite o codigo:\n");
    scanf("%s", codigo1);

    printf("Digite a população: \n");
    scanf("%d", &populacao1);

    printf("Digite a área: \n");
    scanf("%f", &area1);

    printf("Digite o PIB: \n");
    scanf("%f", &pib1);

    printf("Digite os pontos turísticos: \n");
    scanf("%d", &pontosturisticos1);
//coletando dados da carta 1


    printf("carta 2\n");

    printf("Digite o Estado: \n");
    scanf("%s", estado2);

    printf("Digite o codigo:\n");
    scanf("%s", codigo2);

    printf("Digite a população: \n");
    scanf("%d", &populacao2);

    printf("Digite a área: \n");
    scanf("%f", &area2);

    printf("Digite o PIB: \n");
    scanf("%f", &pib2);

    printf("Digite os pontos turísticos: \n");
    scanf("%d", &pontosturisticos2);
//coletanto dados da carta 2

    densidade_populacional1 = populacao1 / area1;
    PIB_per_capita1 = pib1 / populacao1;

    densidade_populacional2 = populacao2 / area2;
    PIB_per_capita2 = pib2 / populacao2;

    super_poder1 = (area1 + pib1 + pontosturisticos1 + densidade_populacional1 + PIB_per_capita1) / 5;
    super_poder2 = (area2 + pib2 + pontosturisticos2 + densidade_populacional2 + PIB_per_capita2) / 5;
//definindo super poder, densidade e pib per capital

    printf("carta1\n");
    printf("Estado: %s\n", estado1);
    printf("Codigo: %s\n", codigo1);
    printf("População: %d\n", populacao1);
    printf("Area: %f\n", area1);
    printf("Pib: %f\n", pib1);
    printf("Pontos turisticos: %d\n", pontosturisticos1);
    printf("Densidade: %f\n", densidade_populacional1);
    printf("PIB per Capita: %f\n", PIB_per_capita1);
    printf("Super poder: %f\n", super_poder1);
//exibindo dados da carta 1


    printf("carta2\n");
    printf("Estado: %s\n", estado2);
    printf("Codigo: %s\n", codigo2);
    printf("População: %d\n", populacao2);
    printf("Area: %f\n", area2);
    printf("Pib: %f\n", pib2);
    printf("Pontos turisticos: %d\n", pontosturisticos2);
    printf("Densidade: %f\n", densidade_populacional2);
    printf("PIB per Capita: %f\n", PIB_per_capita2);
    printf("Super poder: %f\n", super_poder2);
    //exibindo dados da carta 2

    printf("1 significa que a carta 1 venceu\n");
    printf("0 significa que a carta 2 venceu\n");
    //explicando como indentificar quem ganhou

    printf("Populacao1 vs Populacao2: %d\n", populacao1 > populacao2);
    printf("Area1 vs Area2: %f\n", area1 > area2);
    printf("Pib1 vs Pib2: %f\n", pib1 > pib2);
    printf("Pontos turisticos1 vs Pontos turisticos2: %d\n", pontosturisticos1 > pontosturisticos2);
    printf("Densidade populacional1 vs Densidade populacional2: %f\n", densidade_populacional1 > densidade_populacional2);
    printf("PIB per Capita1 vs PIB per Capita2: %f\n", PIB_per_capita1 > PIB_per_capita2);
    printf("Super poder 1 vs Super poder 2: %f\n", super_poder1 > super_poder2);
    //exibindo os resultados




    return 0;
}
