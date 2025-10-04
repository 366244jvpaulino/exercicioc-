

//Faça um algoritmo que leia as respostas de três questões de múltipla escolha (‘a’, ‘b’, ‘c’, ‘d’). Em seguida, leia o gabarito dessas respostas, ou seja, as respostas corretas. Depois, compare as respostas dadas com as do gabarito e indique quantas respostas//



#include <iostream>
using namespace std;

int main() {
char respostas[3];
char gabarito[3];
int acertos = 0;

cout << "Digite as respostas do aluno (a, b, c ou d):" << endl;
for (int i = 0; i < 3; i++) {
cout << "Questao " << (i + 1) << ": ";
cin >> respostas[i];
}

cout << "\nDigite o gabarito oficial (a, b, c ou d):" << endl;
for (int i = 0; i < 3; i++) {
cout << "Gabarito questao " << (i + 1) << ": ";
cin >> gabarito[i];
}


for (int i = 0; i < 3; i++) {
if (respostas[i] == gabarito[i]) {
acertos++;
}
}

cout << "\nO aluno acertou " << acertos << " questao(oes)." << endl;

return 0;
}




