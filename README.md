# Matrizes
//1)

    #include <stdio.h>

    int main() 
    {
    
    int matriz[3][3];
    int i, j;

    printf("Digite os elementos da matriz 3x3:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Elemento [%d][%d]: ", i, j);
            scanf("%d", &matriz[i][j]);
        }
    }

    printf("Matriz 3x3:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d ", matriz[i][j]);
        }
        printf("\n");
    }

    return 0;}

//2)

    #include <stdio.h>

    int main() 
    {
    
    int matriz[3][3];
    int matrizMultiplicada[3][3];
    int i, j;

    printf("Digite os elementos da matriz 3x3:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Elemento [%d][%d]: ", i, j);
            scanf("%d", &matriz[i][j]);
        }
    }

    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            matrizMultiplicada[i][j] = matriz[i][j] * 2;
        }
    }
    printf("Matriz resultante (multiplicada por 2):\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("%d ", matrizMultiplicada[i][j]);
        }
        printf("\n");
    }
    return 0;}

//3)

    #include <stdio.h>

    int main() 
    {
    
    int matriz[2][3];
    int i, j, soma = 0;

    printf("Digite os elementos da matriz 2x3:\n");
    for (i = 0; i < 2; i++) {
        for (j = 0; j < 3; j++) {
            printf("Elemento [%d][%d]: ", i, j);
            scanf("%d", &matriz[i][j]);
            soma += matriz[i][j];
        }
    }

    printf("A soma dos números é: %d\n", soma);

    return 0;}

//4)

    #include <stdio.h>

    int main() 
    {
    
    int matriz[4][4];
    int i, j;

    printf("Digite os elementos da matriz 4x4:\n");
    for (i = 0; i < 4; i++) {
        for (j = 0; j < 4; j++) {
            printf("Elemento [%d][%d]: ", i, j);
            scanf("%d", &matriz[i][j]);
        }
    }

    printf("Elementos da diagonal principal:\n");
    for (i = 0; i < 4; i++) {
        printf("%d ", matriz[i][i]);
    }
    printf("\n");

    return 0;}

//5)

    #include <stdio.h>

    int main() 
    {
    
    int matriz[3][3];
    int i, j;

    printf("Digite os elementos da matriz 3x3:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            printf("Elemento [%d][%d]: ", i, j);
            scanf("%d", &matriz[i][j]);
        }
    }

    printf("Elementos, exceto os da diagonal principal:\n");
    for (i = 0; i < 3; i++) {
        for (j = 0; j < 3; j++) {
            if (i != j) {
                printf("%d ", matriz[i][j]);
            }
        }
    }
    printf("\n");

    return 0;}
