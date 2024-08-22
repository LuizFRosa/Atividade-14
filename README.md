# Atividade-14

#include <stdio.h>

int inverterNumero(int num) {
    int invertido = 0;
    
    while (num != 0) {
        int digito = num % 10;
        invertido = invertido * 10 + digito;
        num /= 10;
    }
    
    return invertido;
}

int main() {
    int numero;
    
    printf("Digite um numero: ");
    scanf("%d", &numero);
    
    int resultado = inverterNumero(numero);
    
    printf("O numero invertido e: %d\n", resultado);
    
    return 0;
}
