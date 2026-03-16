#include <iostream>

using namespace std;

struct Punto {
    float x, y;
};

int main() {

    float* p;

    float v[3] = {1.2, 19, 6};

    float f = 4;

    Punto punto = {2.6, 6};

    // apuntando al atributo x de la estructura
    p = &punto.x;

    // apuntando al segundo elemento del arreglo
    p = &v[1];

    // apuntando a la variable f
    p = &f;

    cout << "La variable f vale: " << f << ", " << *p << endl;

    // modificar el valor usando el puntero
    *p = 5.5;

    cout << "La variable f vale: " << f << endl;

    return 0;
}
