# exerciciocmaismais
**primeiro codigo**
#include <iostream>

using namespace std;

int main()
{
cout << "Repetição com Do-While \n";
cout << endl;

int op; //não posso colocar a variavel dentro da estrutura de repetição//


do {
cout << "**************MENU************ \n";
cout << "* 1 - Cadastro * \n";
cout << "* 2 - Consulta * \n";
cout << "* 3 - Sair * \n";
cout << "****************************** \n";
cout << "* Escolha uma opção: * \n";
cin >> op;

switch(op){
case 1 :
cout << "Cadastrando... \n";
break;
case 2 :
cout << "Consultando... \n";
case 3 :
cout << "Saindo... \n";
break;
} //final do switch
}while (op != 3);








return 0;
}
