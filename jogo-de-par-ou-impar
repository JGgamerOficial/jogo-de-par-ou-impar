#include <stdio.h>
#include <stdlib.h>
#include <time.h>  // Biblioteca para gerar números aleatórios

int main() {
    // Declaração das variáveis
    int computador, jogador;

    // Exibição do menu de opções para o jogador
    printf("\n*** Bem vindo ao Pedra-papel-tesoura ***\n");
    printf("Voce jogara contra o computador....\n");
    printf("Escolha sua jogada:\n");
    printf("1 - Tesoura\n");
    printf("2 - Papel\n");
    printf("3 - Pedra\n");
    printf("Sua jogada: ");
    
    // Captura da jogada do jogador
    scanf("%d", &jogador);

    // Geração do número aleatório para a jogada do computador
    srand(time(NULL));  // Inicializando o gerador de números aleatórios
    computador = 1 + (rand() % 3);  // Gerando um número aleatório entre 1 e 3

    // Exibe a jogada do computador
    printf("O computador jogou: %d\n", computador);

    // Verificação da jogada do jogador
    if (jogador < 1 || jogador > 3) {
        printf("Jogada invalida!!\n");  // Verifica se a jogada do jogador está fora do intervalo válido
    } else {
        // Comparação das jogadas para determinar o resultado
        if (jogador == computador) {
            printf("Empate!!\n");  // Caso as jogadas sejam iguais, há um empate
        } else {
            // Jogada do jogador é Tesoura (1)
            if (jogador == 1 && computador == 2) {
                printf("Voce venceu!!\n");  // Tesoura ganha do papel
            } else if (jogador == 1 && computador == 3) {
                printf("Voce perdeu!!\n");  // Tesoura perde para a pedra
            }

            // Jogada do jogador é Papel (2)
            if (jogador == 2 && computador == 1) {
                printf("Voce perdeu!!\n");  // Papel perde para a tesoura
            } else if (jogador == 2 && computador == 3) {
                printf("Voce ganhou!!!\n");  // Papel ganha da pedra
            }

            // Jogada do jogador é Pedra (3)
            if (jogador == 3 && computador == 1) {
                printf("Voce perdeu!!!\n");  // Pedra perde para o papel
            } else if (jogador == 3 && computador == 2) {
                printf("Voce ganhou!!!\n");  // Pedra ganha da tesoura
            }
        }
    }

    // Finaliza o jogo
    printf("Fim do jogo!!!\n");
    return 0;
}
