# Atividade-SuperTrunfo1
```
#include <stdio.h>

int main () {

    char estado1 = 'A';
    char estado2 = 'B';
    char codigo1 [5] = "A01";
    char codigo2 [5] = "B02";
    char nomeCidade1 [50] = "Recife";
    char nomeCidade2 [50] = "Curitiba";
    unsigned long int populacao1 = 1537704;
    unsigned long int populacao2 = 1751907;
    float area1 = 217.0;
    float area2 = 435.0;
    float PIB1 = 123000000000;
    float PIB2 = 193000000000;
    int pontosTuristicos1 = 15;
    int pontosTuristicos2 = 40;
    float densidade1, densidade2;
    float PIB_percapta1, PIB_percapta2;
    float SuperPoder1, SuperPoder2;

    
    printf ("Carta 1:\n");
    printf ("Estado: %c\n", estado1);
    printf ("Código: %s\n", codigo1);
    printf ("Nome da cidade: %s\n", nomeCidade1);
    printf ("População: %lu\n", populacao1);
    printf ("Área: %f km2 \n", area1);
    printf ("PIB: %.2f bilhões de reais \n", PIB1);
    printf ("Número de Pontos Turísticos: %d\n", pontosTuristicos1);
    
    // Para que não haja perda de dados, utilizar a conversão explícita
    densidade1 = (float) populacao1 / area1;
    printf ("Densidade Populacional: %.2f habitantes/km2\n", densidade1);

    // Para que não haja perda de dados, utilizar a conversão explícita 
    PIB_percapta1 = (float) PIB1 / populacao1;
    printf ("PIB per Capta: %.2f reais\n", PIB_percapta1);

    //Super Poder ( preciso colocar a conversao explicita? )
    SuperPoder1 = (float) populacao1 + area1 + PIB1 + pontosTuristicos1 + PIB_percapta1 + (1 / densidade1);
    printf ("Super Poder: %.2f\n", SuperPoder1);
    



    printf ("Carta 2:\n");
    printf ("Estado: %c\n", estado2);
    printf ("Código: %s\n", codigo2);
    printf ("Nome da cidade: %s\n", nomeCidade2);
    printf ("População: %lu\n", populacao2);
    printf ("Área: %f km2 \n", area2);
    printf ("PIB: %.2f bilhões de reais \n", PIB2);
    printf ("Número de Pontos Turísticos: %d\n", pontosTuristicos2);

    // Para que não haja perda de dados, utilizar a conversão explícita
    densidade2 = (float) populacao2 / area2;
    printf ("Densidade Populacional: %.2f habitantes/km2\n", densidade2);

    // Para que não haja perda de dados, utilizar a conversão explícita
    PIB_percapta2 = (float) PIB2 / populacao2;
    printf ("PIB per Capta: %.2f reais\n", PIB_percapta2);

    //Super Poder ( preciso colocar a conversao explicita? )
    SuperPoder2 = (float) populacao2 + area2 + PIB2 + pontosTuristicos2 + PIB_percapta2 + (1 / densidade2);
    printf ("Super Poder: %.2f\n", SuperPoder2);




    // Comparação das variáveis

    printf ("Resultado Final:\n");

    printf ("População: Carta 1 venceu %d\n", populacao1>populacao2);

    printf ("Área: Carta 1 venceu %d\n", area1>area2);

    printf ("PIB: Carta 1 venceu %d\n", PIB1>PIB2);

    printf ("Pontos Turisticos: Carta 1 venceu %d\n", pontosTuristicos1>pontosTuristicos2);

    printf ("Densidade Populacional: Carta 2 venceu %d\n", densidade2<densidade1);

    printf ("PIB per Capita: Carta 1 venceu %d\n", PIB_percapta1>PIB_percapta2);

    printf ("Super Poder: Carta 1 venceu %d\n", SuperPoder1>SuperPoder2);



}
```
