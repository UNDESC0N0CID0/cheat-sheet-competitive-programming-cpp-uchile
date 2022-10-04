# cheat-sheet-competitive-programming-cpp-uchile
Este repositorio contiene algunos fragmentos de códigos que me pueden ser útiles en la competencia de programación progcomp de uchile


# Operadores Bitwise

## Operadores bitwise

```
#include <iostream>
#include <bitset>

int main()
{
    std::string binary = std::bitset<8>(128).to_string(); //Trasnformamos un número a binario
    std::cout<<Binario<<"\n";

    unsigned long decimal = std::bitset<8>(binary).to_ulong();
    std::cout<<Decimal<<"\n";
    return 0;
}
```
