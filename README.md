Reto #3
A continuación estarán los pseudocódigos y diagramas de flujo para dos distintos problemas.
1. Hallar los números primos hasta n:
función encontrarPrimos(n)
-Pseudocódigo: 
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

fin función
Digrama de flujo: 
[![](https://i.postimg.cc/rpS3mK7P/Captura-de-pantalla-2024-03-05-220220.png)](https://i.postimg.cc/rpS3mK7P/Captura-de-pantalla-2024-03-05-220220.png)

2. Hallar raíces cuadradas (divisiones y restas)
Pseudocódigo:
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
[![](https://i.postimg.cc/BQ42vrbT/Captura-de-pantalla-2024-03-05-220925.png)](https://i.postimg.cc/BQ42vrbT/Captura-de-pantalla-2024-03-05-220925.png)
