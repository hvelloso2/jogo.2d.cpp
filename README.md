#include <iostream>

using namespace std;


 
int main()
{
    int oper;
    char mapa_1 [25][25];
    int j,i;

    cout << "#################################################################################\n";
    cout << "#################################################################################\n";
    cout << "                          BEM VINDO                                              \n";
    cout << "1.jogar.\n";
    cout << "2.tutorial.\n";
    cout << "3.sair.\n";
    cin >> oper;

    switch (oper)
    {
    case 1:
        system("cls");
        for (i = 0; i < 25; i++)
        {   
            
            for(j = 0; j < 25; j++)
            {
                if(i == 0)
                {
                    mapa_1 [i][j] = '*';
                }
                else if(j == 0)
                {
                    mapa_1 [i][j] = '*';
                }
                else if(i == 24)
                {
                    mapa_1 [i][j] = '*';
                }
                else if(j == 24)
                {
                    mapa_1 [i][j] = '*';
                }
                else
                {
                    mapa_1 [i][j] = ' ';
                }
                cout << mapa_1[i][j];
            }
        }

        break;

    case 2:

        system("cls");
        cout << "O jogo é do estilo aventura/puzzle onde o objetivo é o jogador conseguir passar de três fases. Em cada fase o jogador deve se movimentar para pegar uma chave para abrir a porta fechada.";
        cout << "\n\nO jogador possui os seguintes comando:\n\n";
        cout << "W: O jogador movimenta uma unidade para cima;\n";
        cout << "A: O jogador movimenta uma unidade para esquerda;\n";
        cout << "S: O jogador movimenta uma unidade para baixo;\n";
        cout << "D: O jogador movimenta uma unidade para direita;\n";
        cout << "I: O jogador interage com o objeto que ele estar em cima.\n";
        cout << "\nO jogo possui os seguintes elementos nas fases:\n\n";
        cout << "&: Simbolo que representa o jogador.\n";
        cout << "*: Simbolo que representa uma parede, o jogador ao se movimentar não pode passar pela parede.\n";
        cout << "@: Simbolo que representa a chave para abrir a porta para finalizar a fase, a porta abre no momento que o jogador interage com a chave.\n";
        cout << "D: Simbolo que representa a porta fechada.\n";
        cout << "=: Simbolo que representa a porta aberta quando o jogador interagiu com a chave.\n";
        cout << "O: Simbolo que representa um botão que o usuário pode interagir, o botão fica no chão e o jogador deve ficar em cima dele para poder interagir.\n";
        cout << "#: Simbolo que representa um espinho. A fase é reiniciada quando o jogador toca no espinho, caso a fase seja reiniciada três vezes, o jogo volta para o menu principal.\n";
        cout << ">: Simbolo que representa um teletransporte. O teletransporte sempre deve vir em par, quando o jogador toca em um ele é transportado para o outro e vice-versa.\n";
        system("pause");
        system("cls");
        break;

    case 3:
        cout << "saindo......";
        system("pause");
        system("cls");
        break;

    default:
        cout << "escolha umas das opcoes validas.\n";
        system("pause");
        system("cls");
        break;
    }

    



}
