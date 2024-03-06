Reto #3
A continuación estarán los pseudocódigos y diagramas de flujo para dos distintos problemas.
1. Hallar los números primos hasta n:

-Pseudocódigo:

```pseudocode
   función encontrarPrimos(n)
    para cada número i desde 2 hasta n hacer
        esPrimo = verdadero
        para cada número j desde 2 hasta la raíz cuadrada de i hacer
            si i mod j == 0 entonces
                esPrimo = falso
                salir del bucle
            fin si
        fin para
        si esPrimo entonces
            imprimir i
        fin si
    fin para
fin función
```


Digrama de flujo:

``` mermaid
graph TD
    A[Inicio] --> B[Establecer n]
    B --> C{Para cada número i = 2 hasta n}
    C -->|Para cada i| D{Para cada j = 2 hasta raíz cuadrada de i}
    D --> E{Si i mod j == 0}
    E -->|Verdadero| F[esPrimo = falso]
    F --> G[Salir del bucle j]
    E -->|Falso| H{Fin del bucle j}
    D --> H
    H --> I{Si esPrimo == verdadero}
    I -->|Verdadero| J[Imprimir i]
    I -->|Falso| K[Continuar con el siguiente i]
    J --> L{Fin del bucle i}
    K --> L
    L --> M[Fin]
```

2. Hallar raíces cuadradas (divisiones y restas)
Pseudocódigo:

```pseudocode
función encontrarRaizCuadrada(n)
    resultado = 0
    odd = 1
    mientras n >= odd hacer
        n = n - odd
        odd = odd + 2
        resultado = resultado + 1
    fin mientras
    retornar resultado
fin función
```

Diagrama de flujo:

``` mermaid
graph TD
    A[Inicio] --> B[Establecer n, resultado = 0, odd = 1]
    B --> C{Mientras n >= odd}
    C -->|Verdadero| D[Restar n = n - odd]
    D --> E[Incrementar odd = odd + 2]
    E --> F[Incrementar resultado = resultado + 1]
    F --> C
    C -->|Falso| G[Retornar resultado]
    G --> H[Fin]
```


