# Explicação do Código

Este código é uma implementação do algoritmo de Euclides para encontrar o maior divisor comum (MDC) de dois números inteiros.

## Inclusão de Bibliotecas

```cpp
#include<bits/stdc++.h>
```
Inclui todas as bibliotecas padrão do C++. Não é recomendado para uso em produção.

## Uso do Espaço de Nomes

```cpp
using namespace std;
```
Permite o uso de funções da biblioteca padrão sem o prefixo `std::`.

## Função gcd

```cpp
int gcd(int a, int b){
    if(a == 0){
        return b;
    }
    return gcd(b % a, a);
}
```
Define a função `gcd` que usa o algoritmo de Euclides para calcular o MDC.

### Condição de Parada

Se `a` for zero, retorna `b` como o MDC.

### Chamada Recursiva

Continua a operação com `b % a` e `a`.

## Função Principal

```cpp
int main()
{
    pair<int, int> teste;
    
    cin >> teste.first >> teste.second;
    
    cout << gcd(teste.first, teste.second);
    
    return 0;
}
```
Define a função `main`, que é o ponto de entrada do programa.

### Par de Inteiros

Cria um par `teste` para armazenar os dois números.

### Entrada do Usuário

Lê dois números inteiros e os armazena em `teste.first` e `teste.second`.

### Saída do Resultado

Imprime o resultado da função `gcd`.

### Retorno de Sucesso

Indica que o programa terminou com sucesso.
