
  //Faça um algoritmo que leia três números e determine quantos são iguais//

#include <iostream>
using namespace std;

int main() {
int a, b, c;
cout << "Digite tres numeros: ";
cin >> a >> b >> c;

if (a == b && b == c) {
cout << "Todos os tres numeros sao iguais." << endl;
} else if (a == b || a == c || b == c) {
cout << "Dois numeros sao iguais." << endl;
} else {
cout << "Todos os numeros sao diferentes." << endl;
}

return 0;
}




//Faça um algoritmo que leia um número inteiro diferente de zero e diga se este é positivo ou negativo.//

#include <iostream>
using namespace std;

int main() {
int numero;


do {
cout << "Digite um número inteiro diferente de zero: ";
cin >> numero;

if (numero == 0) {
cout << "Erro: o número não pode ser zero. Tente novamente." << endl;
}
} while (numero == 0);


if (numero > 0) {
cout << "O número é positivo." << endl;
} else {
cout << "O número é negativo." << endl;
}

return 0;
}


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



//Faça um algoritmo que solicite ao usuário o ano em que nasceu e o ano atual, feito isso o programa irá calcular a idade do usuário, se ele tiver 16 anos ou mais o programa deverá mostrar a mensagem “Você pode votar”, porém se ele possuir idade inferior a 16 anos o programa deverá calcular a diferença, ou seja, quantos anos faltam para ele completar 16 anos e depois mostrar a mensagem “Você ainda não pode votar, deve esperar mais ” diferença de anos//





#include <iostream>
using namespace std;
int main (){
int anoatual,anonascimento,idade;

cout<<"informe o ano atual:";
cin>>anoatual;

cout<<"informe o ano de nascimento:";
cin>>anonascimento;

idade=anoatual-anonascimento;
if(idade>=18){
    cout<< "voce ja pode votar\n";
}else{
cout<<"voce nao pode votar";

}



return 0;
}


















