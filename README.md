# atv-iago

Atv 1 
```C
1 - #include <stdio.h>

int main() {
    int matriz[2][2] = {
        {10, 20},
        {30, 40}
    };

    printf("Matriz 2x2 com os números 10, 20, 30, 40:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++)
            printf("%d ", matriz[i][j]);
        printf("\n");
    }

    return 0;
}
```

Atv 2 
```C
2 - #include <stdio.h>

int main() {
    int matriz[4][4] = {
        {1, 2, 3, 4},
        {5, 6, 7, 8},
        {9, 10, 11, 12},
        {13, 14, 15, 16}
    };
    printf("Matriz 4x4:\n");
    for (int i = 0; i < 4; i++) {
        for (int j = 0; j < 4; j++)
            printf("%d ", matriz[i][j]);
        printf("\n");
    }

    printf("\nDiagonal principal:\n");
    for (int i = 0; i < 4; i++)
        printf("%d ", matriz[i][i]);

    printf("\n");
    return 0;
}
```

Atv 3
```C
3 - #include <stdio.h>

int main() {
    int matriz[2][3] = {
        {1, 2, 3},
        {4, 5, 6}
    };
    int soma_total = 0;
    printf("Matriz 2x3:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++) {
            printf("%d ", matriz[i][j]);
            soma_total += matriz[i][j];
        }
        printf("\n");
    }

    printf("Soma de todos os elementos: %d\n", soma_total);
    return 0;
}
```

Atv 4
```C
4 - #include <stdio.h>

int main() {
    int matriz[3][3] = {
        {2, 10, 5},
        {9, 1, 3},
        {4, 6, 150}
    };
    int maior_valor = -2147483648; // Valor mínimo para int

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (matriz[i][j] > maior_valor) {
                maior_valor = matriz[i][j];
            }
        }
    }

    printf("O maior valor na matriz é: %d\n", maior_valor);
    return 0;
}
```

Atv 5
```C
5-  #include <stdio.h>

int main() {
    int matriz[3][2] = {
        {1, 5},
        {8, 3},
        {4, 9}
    };
    int contagem_pares = 0;
    for (int i = 0; i < 3; i++)
        for (int j = 0; j < 2; j++)
            if (matriz[i][j] % 2 == 0)
                contagem_pares++;

    printf("Total de números pares na matriz: %d\n", contagem_pares);
    return 0;
}
```

Atv 6
```C
6 - #include <stdio.h>

int main() {
    int matriz[2][2] = {
        {10, 20},
        {30, 40}
    };
    int temp;

    // Troca as linhas
    for (int j = 0; j < 2; j++) {
        temp = matriz[0][j];
        matriz[0][j] = matriz[1][j];
        matriz[1][j] = temp;
    }

    printf("Matriz com linhas trocadas:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++)
            printf("%d ", matriz[i][j]);
        printf("\n");
    }

    return 0;
}
```

Atv 7
```C
7 - #include <stdio.h>

int main() {
    int matriz[2][3] = {
        {100, 200, 300},
        {400, 500, 600}
    };
    printf("Matriz 2x3:\n");
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++)
            printf("%d\t", matriz[i][j]);
        printf("\n");
    }

    return 0;
}
```

Atv 8 
```C
8 - #include <stdio.h>

int main() {
    int matriz[3][3] = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9}
    };
    int soma_linha;
    for (int i = 0; i < 3; i++) {
        soma_linha = 0;
        for (int j = 0; j < 3; j++)
            soma_linha += matriz[i][j];
        printf("Soma da linha %d: %d\n", i + 1, soma_linha);
    }

    return 0;
}
```

Atv 9
```C
9 - #include <stdio.h>

int main() {
    int matriz_original[2][3] = {
        {10, 20, 30},
        {40, 50, 60}
    };
    int transposta[3][2];

    // Gera a transposta
    for (int i = 0; i < 2; i++)
        for (int j = 0; j < 3; j++)
            transposta[j][i] = matriz_original[i][j];

    // Exibe a transposta
    printf("A matriz transposta (3x2) é:\n");
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 2; j++)
            printf("%d\t", transposta[i][j]);
        printf("\n");
    }

    return 0;
}
```
