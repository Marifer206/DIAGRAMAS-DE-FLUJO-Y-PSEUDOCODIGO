# DIAGRAMAS DE FLUJO Y PSEUDOCODE 🚀
## RETO 4
 - Plantear el algoritmo para obtener los números primos hasta n, usando pseudocódigo y diagramas de flujo
 - Revise el procedimiento matemático para hallar raices cuadradas (son divisiones y restas), plantee el algoritmo en pseudocódigo y en diagrama de flujo.

### NUMEROS PRIMOS EN UN LISTA DE NUMEROS HASTA N
Este codigoo funciona pondiendo condiciones las cuales iterara en cada numero de la lista para seleccionarlos o imprimir como numeros primos, las condiciones son que no sea igual o menor que 1 y que el residuo de su dividon con algun numero en el rango de 2 a la √n+1, este rango se hace para que pueda tomar todos los valores incuyendo el de su raiz propia, en el codigoo se utilizaria una libreria para usar math.sqrt para sacar las raices.

#### PSEUDOCODE
```pseudocode
[variables]
  n: entero
  i: entero
  x: entero
  
Inicio
  n: es_primo
   Si n <= 1: no es primo 
   Para cada numero i tomar un valor del rango del 2 a la raiz de n + 1 
   Si n % 1 == 0 : no es primos
   
 Hacer la lista de numeros n
 Hacer la lista de numeros n primos
 
 Para cada número "x" en la lista "numeros n" se debe 
    Si "x" es_primo entonces agregarlo a la lista "numeros n primos"

Imprimir la lista "numeros n primos"

Fin
  
```
#### DIAGRAMAS DE FLUJO
```mermaid
graph TD;
    A(Inicio) --> B[Definir variables n:entero i:entero x:entero]
    B --> C[n: es_primo] --> D{n es mayor que 1}
    D --> |Si|E{la division de n por algun numero del rango de 2 a la raiz de n + 1 da un residuo igual a 0}
    D --> |No|F[no es un numero primo]
    E --> |No|G[es un numero primo] --> H[Definir los numeros de lista de numeros ''n'']
    E --> |si|F[no es un numero primo]
    H --> J[crear lista numeros ''n'' primos]
    J --> I[a cada número ''x'' en la lista numeros ''n'' hacer o remplazar en n:es_primo]
    I --> K[Si X es_primo poner en la lista de numeros ''n''primos]
    K --> L[impimir la lista de numeros ''n'' primos]
    L --> M(Fin)

```

### RAICES CUARADAS 
El método de la bisección es un algoritmo de búsqueda que se utiliza para encontrar el cero (o raíz) de una función. El algoritmo comienza con un intervalo que contiene la raíz y lo divide sucesivamente a la mitad hasta que se alcanza la precisión deseada.

#### PSEUDOCODE
```pseudocode
[variables]
n: real positivo
y: entero
precision:
Incio
Algoritmo raiz_cuadrada (n)
Se inicializan las variables
    x = n
    y = 1
    precisión = 0.000001

    mientras (x - y > precisión) hacer:
        x = (x + y) / 2
        y = n / x

    devolver x
n= numero que da el usuario que quiera sacar su raiz
print(raiz_cuadrada(n))
Fin

```
#### DIAGRAMAS DE FLUJO
```mermaid
graph TD;
       A(Inicio) --> B[Inicializar x = n, y = 1]
    B --> K[Dar valor a n el numero que se quiera saber la raiz ejm:25]
    K --> C[Establecer la precisión deseada ejm:0.00001] 
    C --> E{ x - y > precision}
    E --> |NO|L[mostrar raiz_cuadrada de ''n''' ejm: 5.000000000053722]-->H(Fin)
    E --> |SI|F[Calcular el valor medio como x + y / 2]
    F --> I[y = n / x]
    I --> J[Actualizar el valor de x e y en función de si el cuadrado del valor medio es mayor o menor que n]
    J --> E

```
