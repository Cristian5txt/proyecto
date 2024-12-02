#include <iostream>
#include <unistd.h> //se utilizo esta libreria para que no se ejecute el codigo todo a la misma vez(sleep)
using namespace std;

int main()
{
    int semaforo1,semaforo2,semaforo3,semaforo4; //declaracion de variables de tipo int

    // declaracion de variables tipo char
    char boton;
    char crusar;


    //GRAFICO DE LA INTERSECCION VIA
    cout <<"           |      |       |"<<endl;
    cout <<"           |      |       |"<<endl;
    cout <<"           |              |"<<endl;
    cout <<"           |      |       |"<<endl;
    cout <<"           |              |"<<endl;
    cout <<"           |      |       |"<<endl;
    cout <<"                          :"<<"              "<<":                          "<<endl;
    cout <<"                         1:"<<"      3       "<<":                          "<<endl;
    cout <<"-----------:"<<"             "<<":------------"<<endl<<endl<<endl;
    cout <<  "_ _ _ "<<"            |      "<<" _ _ _"<<endl<<endl<<endl;

    cout <<"-----------"<<"       |       "<<"-----------"<<endl;
    cout <<"                          :"<<"              "<<":2                          "<<endl;
    cout <<"                          :"<<"      4        "<<":                          "<<endl;
    cout <<"                          :"<<"              "<<":                          "<<endl;
    cout <<"           |      |       |"<<endl;
    cout <<"           |      |       |"<<endl;
    cout <<"           |              |"<<endl;
    cout <<"           |      |       |"<<endl;
    cout <<"           |              |"<<endl;
    cout <<"           |      |       |"<<endl;

    //Mensaje de los estados del semaforo
    cout << "ESTADO DE LOS SEMAFOROS " << endl<<endl<<endl;
    sleep(1.5);                     //EL SLEEP ES COMO UN DELAY
    do{                             // SE REALIZO UN DO-WHILE PARA NUESTRO CODIGO SE PUEDA EJECUTAR EN EL BUCLE
        do{                         // SE REALIZO OTRO DO-WHILE PARA QUE SE EJECUTE UN BUCLE PARA VER SI SE PUEDE CRUZAR O NO
    cout <<"semaforo_1"<<endl<<endl;
    sleep(1.5);
    cout <<"verde"<<endl<<endl;
    sleep(1.5);
    cout <<"semaforo_2"<<endl<<endl;
    sleep(1.5);
    cout <<"verde"<<endl<<endl;
    sleep(1.5);
    cout <<"semaforo_3"<<endl<<endl;
    sleep(1.5);
    cout <<"rojo"<<endl<<endl;
    sleep(1.5);
    cout <<"semaforo_4"<<endl<<endl;
    sleep(1.5);
    cout <<"rojo"<<endl<<endl;
    sleep(1.5);
    cout <<"desea crusar y/n"<<endl; //MENSAJE DE QUE SI SE PUEDE CRUZAR O NO
    cin>> crusar;                    //INGRESAR EL VALOR DE Y o N
}while(crusar=='n');

    cout<<"presione (1) para activar el boton,presione (0) para no precionarlo  "<<endl<<endl; //MENSAJE DE PEDIR EL VALOR DE 1 o 0 PARA EL BOTON
    cin>>boton;                                                                                //INGRESAR EL VALOR DEL BOTON
    if (boton=='1'){     // SI EL VALOR ES == 1 SE EJECUTA TODO LO INDICADO
        cout<<"semaforo1"<<endl;
        sleep(1.5);
        cout<<"amarillo"<<endl;
        sleep(2.5);
        cout<<"rojo"<<endl<<endl;

        cout<<"semaforo2"<<endl;
        sleep(1.5);
        cout<<"amarillo"<<endl;
        sleep(2.5);
        cout<<"rojo"<<endl<<endl;

        cout<<"semaforo3"<<endl;
        sleep(1);
        cout<<"verde"<<endl;

        cout<<"semaforo4"<<endl;
        sleep(1);
        cout<<"verde"<<endl<<endl;
        cout<<"puedes crusar"<<endl<<endl;
        sleep(5);

    }

    }while(1);
    return 0;
}
