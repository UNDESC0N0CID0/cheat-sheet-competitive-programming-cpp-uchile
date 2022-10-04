# cheat-sheet-competitive-programming-cpp-uchile
Este repositorio contiene algunos fragmentos de códigos que me pueden ser útiles en la competencia de programación progcomp de uchile


# Operadores Bitwise

### LEFT SHIFT
(x<<y)' es equivalente a multiplicar x por 2^y (2 elevado a la potencia y). 
Ej.: x<<y (x: primer operando, y: segundo operando)

Toma dos números, desplaza a la izquierda los bits del primer operando, el segundo operando decide el número de lugares a desplazar.
```
00000000 00000000 00000000 00000110
```
Desplazar este patrón de bits a la izquierda una posición ( 6 << 1) daría como resultado el número 12:

```
00000000 00000000 00000000 00001100
```
## Mostrar números en base 2 y base 10

```
#include <iostream>
#include <bitset>

int main()
{
    std::string binary = std::bitset<8>(128).to_string(); //Desplegamos el 128 en base 2
    std::cout<<Binario<<"\n";

    unsigned long decimal = std::bitset<8>(binary).to_ulong();
    std::cout<<Decimal<<"\n";
    return 0;
}
```
