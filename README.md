# DIAGRAMAS-DE-FLUJO-Y-PSEUDOCODE
## RETO 4
 - Plantear el algoritmo para obtener los números primos hasta n, usando pseudocódigo y diagramas de flujo
 - Revise el procedimiento matemático para hallar raices cuadradas (son divisiones y restas), plantee el algoritmo en pseudocódigo y en diagrama de flujo.

### NUMEROS PRIMOS EN UN LISTA DE NUMEROS HASTA N
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
#### PSEUDOCODE
```pseudocode
[variables]

  
Inicio
 

Fin
  
```
#### DIAGRAMAS DE FLUJO
```mermaid
graph TD;
   

```
