# <h1 align="center"> Desafios </h1>

## ```Desafio 1 ```[Resolución](#Desafio_1)

* Queremos ingresar un número desde teclado e imprimir si el número es o no par.
* ¿Cómo sería el pseudocódigo de esto?
```
Ingresar un número desde teclado
SI es par: 
    Mostrar mensaje: "es par"
SINO:
    Mostrar mensaje: "NO es par"
```
## ```Desafio 2``` [Resolución](#Desafio_2)
* Queremos ingresar un número desde el teclado e imprimir si es múltiplo de 2,3 o 5.
* **Pista**: Python tiene otra forma de la sentencia condicional: if-elif-else

## ```Desafio 3``` [Resolución](#Desafio_3)
* Dado una letra ingresada por el teclado, queremos saber si es mayúscula o minúscula.

## ```Desafio 4 ```[Resolución](#Desafio_4)
* Dado un caracter ingresado por el teclado, queremos saber si es una comilla o no.
¿Hay algún problema?

## ```Desafio 5``` [Resolución](#Desafio_5)
* Dadas dos cadenas ingresadas desde el teclado, imprimir aquella que tenga más caracteres.

## ```Desafio 6``` [Resolución](#Desafio_6)
* Escribir un programa que ingrese desde teclado una cadena de caracteres e imprima cuántas letras a contiene.

## ```Desafio 7``` [Resolución](#Desafio_7)
* Escribir un programa que ingrese 4 palabras desde teclado e imprima aquellas que contienen la letra r.
* **Pensar**: ¿Podemos usar la instrucción for tal cual la vimos la clase pasada para las 4 iteraciones?
* La sentencia for permite iterar sobre una secuencia.

## ```Desafio 8 ```[Resolución](#Desafio_8)
* Vamos a modificar el código anterior para que imprima la cadena R si la palabra contiene la letra r y sino, imprimal NO TIENE R

## ```Desafio 9 ```[Resolución](#Desafio_9)
* Ingresar palabras desde teclado hasta ingresar la palabra FIN. Imprimir aquellas que empiecen y terminen con la misma letra

* ¿Qué estructura de control deberiamos utilizar para realizar esta interación?¿Podemos utilizar la sentencia for?

## ```Desafio 10 ```[Resolución](#Desafio_10)
**Necesitamos procesar las notas de los estudiantes de este curso. Queremos saber:**

* Cuál es el promedio de las notas
* Cuántos estudiantes están por debajo del promedio
```
Ingresar las notas
Calcular el promedio
Calcular cuántos tienen notas menores al promedio

```
* Empecemos con el primer proceso: vamos a suponer que ingresamos datos hasta que ingrese una nota -1

## ```Desafio 11 ```[Resolución](#Desafio_11)
**Necesitamos procesar las notas de los estudiantes de este curso. Queremos saber:** 

* ¿Cúal es el promedio de las notas?
* ¿Qué estudiantes están por debajo del promedio?
* ¿Qué diferencia hay con el desafio anterior?

* Deberíamos ingresar no sólo las notas, sino también los nombres de los estudiantes.
¿Qué soluciones proponen?

## ```Desafio 12 ```[Resolución](#Desafio_12)
**Queremos escribir una función que imprima sus argumentos agregando de qué tipo son**

* Por ejemplo, podríamos invocarla de la siguiente manera:
```
imprimo(1) --> 1 es de tipo <class 'int'>
imprimo(2, "hola") --> 2 es de tipo <class 'int'>, hola es de tipo <class 'str'>
imprimo([1,2], "hola", 3.2) --> [1, 2] es de tipo <class 'list', hola es de tipo <class 'str'>
```

## ```Desafio 13 ```[Resolución](#Desafio_13)
**Queremos implementar una función que dada una cadena de texto, retorne las palabras que contiene en orden alfabético.**

## ```Desafio 14 ```[Resolución](#Desafio_14)
**Queremos implementar una función que dada una colección con datos de usuarios de un determinado juego (por ejemplo nombre, nivel y puntaje), queremos retornar esta colección ordenada de acuerdo al nombre.**

## ```Desafio 15 ```[Resolución](#Desafio_15)
**Usando expresiones lambda escribir una función que permita codificar una frase según el siguiente algoritmo:**
```
encripto("a") --> "b"
encripto("ABC") --> "BCD"
encripto("Rock2021") --> "Spdl3132"
```

## ```Desafio 16 ```[Resolución](#Desafio_16)
**Dado el conjunto de datos con series y películas de Netflix, queremos:**
* 1. guardar en otro archivo las peliculas agregadas en el año 2021.
* 2. los cinco (5) países con más producciones en Netflix.

# Desafio_1
```Py
num=int(input("Ingrese un numero: "))
if num % 2 == 0:
    print("Es PAR")
else:
    print("Es IMPAR")
```
# Desafio_2
```Py
num=int(input("Ingrese un numero: "))
if num % 2 == 0:
    print("Es multiplo de 2")
elif num % 3 == 0:
    print("Es mulitplo de 3")
elif num % 5 == 0:
    print("Es multiplo de 5")
else:
    print("No es multiplo de 2, 3 o 5")
```
# Desafio_3
```Py
letra=input("Ingrese una letra: ")
if ((letra >="a") and (letra<="z")):
    print("Es minuscula")
elif ((letra >="A") and (letra<="z")):
    print("Es mayuscula")
else:
    print("No es una letra")
```
# Desafio_4
```Py
caracter=input("Ingrese un caracter: ")
if caracter=="\"":
    print("El caracter es una comilla")
else:
    print("No es comilla")
```
# Desafio_5
```Py
cadena1=input("Ingrese la primera cadena: ")
cadena2=input("Ingrese la segunda cadena: ")
if len(cadena1)>len(cadena2):
    print("La cadena \""+cadena1+"\" tiene mas caracteres que la cadena \""+cadena2+"\"")
elif len(cadena1)<len(cadena2):
    print("La cadena \""+cadena2+"\" tiene mas caracteres que la cadena \""+cadena1+"\"")
else: 
    print("Las cadenas tienen la misma cantidad de caracteres")
```

# Desafio_6
```Py
cadena=input("Ingrese cadena a contar sus letras \"a\": ")
contador=0
for c in cadena:
    if (c=="a"):
        contador+=1
print("Cantidad de letras \"a\" en "+cadena+" es: ",contador)
```

# Desafio_7
```Py
for c in range(4):
    cadena=input("Ingrese una cadena: ")
    if "r" in cadena:
        print("La cadena \"{}\" contiene r".format(cadena))
```

# Desafio_8
```Py
for c in range(4):
    cadena=input("Ingrese cadena")
    if "r" in cadena:
        print("TIENE R")
    else:
        print("NO TIENE R")
```

# Desafio_9
```Py
cadena=input("Ingrese una palabra: ")
while cadena != "FIN":
    if cadena[0]== cadena[len(cadena)-1]:
        print(cadena+" empieza y termina con la misma letra")
    else:
        print(cadena+" no empieza y termina con la misma letra")
    cadena=input("Ingrese una palabra: ")
```

# Desafio_10
```Py
nota = int(input("Ingresá una nota (-1 para finalizar): "))
acumulador=0
lista_de_notas = []

while nota != -1:
    acumulador+=nota
    lista_de_notas.append(nota)
    nota = int(input("Ingresá una nota (-1 para finalizar): "))

promedio=acumulador/len(lista_de_notas)

estudiantes_debajo_promedio=0

for indice in range(len(lista_de_notas)):
    if lista_de_notas[indice]<promedio:
        estudiantes_debajo_promedio+=1


print("Promedio de notas: {:.2f}".format(promedio))
print("Cantidad de estudiantes por debajo del promedio: ",estudiantes_debajo_promedio)
```

# Desafio_11
```Py
def ingreso_notas():
    nombre = input("Ingresa un nombre (<FIN> para finalizar): ")
    dicci = {}
    while nombre != "FIN":
        nota = int(input(f"Ingresa la nota de {nombre}: "))
        dicci[nombre] = nota
        nombre = input("Ingresa un nombre (<FIN> para finalizar): ")
    return dicci

notas_de_estudiantes=ingreso_notas()

acumulador=0
for n in notas_de_estudiantes.values():
    acumulador+=n
promedio= 0 if len(notas_de_estudiantes)==0 else acumulador/len(notas_de_estudiantes)
estudiantes_debajo_promedio = []
for alumno in notas_de_estudiantes:
    if notas_de_estudiantes[alumno]<promedio:
        estudiantes_debajo_promedio.append(alumno)

print("Promedio de notas: {:.2f}".format(promedio))
print("Lista de estudiantes por debajo del promedio ")
for elem in estudiantes_debajo_promedio:
    print(elem+"\n")
```
# Desafio_12
```Py
def imprimo(*args):
    for i in range(len(args)):
        print(f'{args[i]} de tipo {type(args[i])}')

imprimo(1) 
imprimo(2, "hola")
imprimo([1,2], "hola", 3.2)
```

# Desafio_13
```Py
def ordeno(cadena):
    """retorna una lista con las palabras de la cadena recibida en orden alfabético
    """
    palabras=cadena.lower().split()
    palabras.sort(key=str.lower)
    return set(palabras)

print(ordeno("Hoy hoy puede ser un gran día. "))
```

# Desafio_14
```Py
def ordeno_usuarios(usuarios):
    """retorna la colección recibida ordenada de acuerdo al nombre.
    """
    return sorted (usuarios,key=lambda usuario: usuario[0])


usuarios = [
('JonY BoY', 'Nivel3', 15),
('1962', 'Nivel1', 12),
('caike', 'Nivel2', 1020),
('Straka^', 'Nivel2', 1020),
]
print(ordeno_usuarios(usuarios))
```

# Desafio_15
```Py
def codigos_ascci(cadena):
    """retorna una lista con strings de los cod ascci de cada caracter de la cadena
    """
    lista=list(map(lambda x:ord(x),cadena))
    return lista


def cifrado_Cesar(cadena):
    """retorna la frase con el siguiente de cada caracter de la misma
    """
    caracteres=codigos_ascci(cadena)
    frase=''.join(map(lambda x:chr(x+1),caracteres))
    return frase


print(cifrado_Cesar('abc'))
#Hecho por la profe
cadena='abc'
cifrado_cesar=map(lambda x: chr(ord(x)+1),cadena)
cifrado_Cesar=''.join(cifrado_Cesar)
print(cifrado_Cesar)
```

# Desafio_16
```Py
import csv
import os
from collections import Counter


ruta_completa =os.getcwd()
ruta_archivo_netflix =os.path.join(ruta_completa, "netflix_titles.csv")
ruta_peliculas_2021=os.path.join(ruta_completa, "peliculas_2021.csv")

archivo_netflix=open(ruta_archivo_netflix, encoding='utf-8')
archivo_peliculas=open(ruta_peliculas_2021,'w',encoding='utf-8')

reader=csv.reader(archivo_netflix, delimiter=',')
writer=csv.writer(archivo_peliculas)
writer.writerow(next(reader))
paises={}

for linea in reader:
    if linea[7]=="2021" and linea[1]=="Movie":
        writer.writerow(linea)
    if linea[5] in paises.keys():
        paises[linea[5]]+=1
    else:
        paises[linea[5]]=1
del paises['']
top_5=dict(Counter(paises).most_common(5))
print('Los 5 paises con más titulos: ')
print(top_5)

archivo_netflix.close()
archivo_peliculas.close()

```

