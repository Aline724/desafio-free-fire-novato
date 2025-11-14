# desafio-free-fire-novato
Desafio: nível novato, primeiros passos na criação do jogo Free Fire, cadastro de itens

#include <stdio.h>
#include <string.h>

#define MAX 10

struct Item {
    char nome[30];
    char tipo[30];
    int quantidade;
};

int main() {
    struct Item mochila[MAX];
    int qtd = 0;
    int opcao;

    do {
        printf("\n===== MOCHILA DE SOBREVIVENCIA =====\n");
        printf("Itens na mochila: %d/%d\n", qtd, MAX);
        printf("1. Adicionar Item\n");
        printf("2. Remover Item\n");
        printf("3. Listar Itens\n");
        printf("0. Sair\n");
        printf("Escolha uma opcao: ");
        scanf("%d", &opcao);
