# Qué es Python?
Python es un lenguaje de programación interpretado cuya filosofía hace hincapié en la legibilidad de su código.​ Se trata de un lenguaje de programación multiparadigma, ya que soporta parcialmente la orientación a objetos, programación imperativa y, en menor medida, programación funcional.


# Qué es una variable?
En Python las variables son "etiquetas" que permiten hacer referencia a los datos (que se guardan en unas "cajas" llamadas objetos).

## Nombrando una variable
le damos de nombrer alguna incial o algo que identifique la accion que vamos hacer 

```python
suma = s 
```

## Asignando valores a una variable
le damos un valor que tiene la variable

```python
num = 0
```

## Operadores básicos
Aqui las operaciones basicas:
### Suma
```python 
suma = num1 + num2
```

### Resta
```python 
res = num1 - num2
```

### Multiplicación
```python 
mul = num1 * num2
```

### División
```python 
div = num1 / num2
```

### Módulo
```python 
div= 5 / 5= 1
```

```python 
mod = 5/ 5= 0
```

# Tipos de datos en Python
En Python todo es un objeto. Así que los tipos de datos serían las clases (donde se definen las propiedades y qué se puede hacer con ellas) y las variables serían las instancias (objetos) de los tipos de datos.

## Integer
Dara el valor entero 

```python
int
division = 9 / 5 = 1
```

## Float
Dara el valor con decimales

```python
int
division = 9 / 5 = 1.8
```

## String
Los cadenas (o strings) son un tipo de datos compuestos por secuencias de caracteres que representan texto. Estas cadenas de texto son de tipo str y se delimitan mediante el uso de comillas simples o dobles.

```python
>>> cadena = "Programa en Python"
>>> cadena[0:8:1]
'Programa'
>>> cadena[12:18:1]
'Python'
```
## Casting en Python
Hacer un cast o casting significa convertir un tipo de dato a otro. Anteriormente hemos visto tipos como los int, string o float. Pues bien, es posible convertir de un tipo a otro.

```python
a = 1   # <class 'int'>
b = 2.3 # <class 'float'>

a = a + b
print(a)       # 3.3
print(type(a)) # <class 'float'>
```

## List
En Python tiene varios tipos de datos compuestos y dentro de las secuencias, están los tipos de cadenas de caracteres. Otro tipo muy importante de secuencia son las listas.

```python
>>> factura = ['pan', 'huevos', 100, 1234]
>>> factura
['pan', 'huevos', 100, 1234]
```

## Tuple
Un tuple es una colección de datos cuyo orden es inalterable, o sea, son elementos ordenados en una secuencia específica y que posee importancia. En Python, los tuples se escriben entre paréntesis.

```python
tuples_frutas=("manzanas, "platano","cereveza")
print(tuple _frutas)
```
## Dictionary
Los diccionarios se utilizan para almacenar valores de datos en pares clave:valor.

```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
```

# Tomando decisiones
si cierta condicion se toma se seguira por esa rama caso contrario se tomara la siguiente rama o se dara fin si ya no hya ramas que coincidan con las condicones.

```python
a = 24
if a % 2 == 0:
    print(a, "is an even number")
b = 23
if b % 2 == 0:
    print(b, "is an odd number")
```

## Sentencia if
En la sentencia if sólo tienes un bloque de sentencias y este bloque se ejecuta sólo cuando la condición es True, se ignora cuando la condición es False.

```python
a = 24
if a % 2 == 0:
    print(a, "is an even number")
b = 23
if b % 2 == 0:
    print(b, "is an odd number")
```
## Ciclo For
El bucle for se utiliza para recorrer los elementos de un objeto iterable (lista, tupla, conjunto, diccionario, …) y ejecutar un bloque de código. En cada paso de la iteración se tiene en cuenta a un único elemento del objeto iterable, sobre el cuál se pueden aplicar una serie de operaciones.

```python
for <elem> in <iterable>:
    <Tu código>
```

## Ciclo While
Un bucle while permite repetir la ejecución de un grupo de instrucciones mientras se cumpla una condición (es decir, mientras la condición tenga el valor True).

```python
i = 1
while i <= 3:
    print(i)
    i += 1
print("Programa terminado")
```

## Break
En Python, la instrucción break le proporciona la oportunidad de cerrar un bucle cuando se activa una condición externa. Debe poner la instrucción break dentro del bloque de código bajo la instrucción de su bucle, generalmente después de una instrucción if condicional.

```python
number = 0

for number in range(10):
    if number == 5:
        break    # break here

    print('Number is ' + str(number))

print('Out of loop')
```
## Continue
La instrucción continueda la opción de omitir la parte de un bucle en la que se activa una condición externa, pero continuar para completar el resto del bucle. Es decir, la iteración actual del bucle se interrumpirá, pero el programa volverá a la parte superior del bucle.

```python
number = 0

for number in range(10):
    if number == 5:
        continue    # continue here

    print('Number is ' + str(number))

print('Out of loop')
```

# Ejercicios 
## for

```python
contador=0
n=5
numero=0
suma =0

for i in range (n):
    numero=int (input ("ingrese numero reales....."))
    
    suma += numero
    contador =contador + 1

if contador == 0:
    print("no digito ningun numero.")

else :
    promedi = suma / contador 

    print("media retimetica es:",promedi)
```

```python
n=5
menor=100000
suma =0

for i in range (n):
    nota=int (input ("ingrese nota:"))
    
    suma += nota
    
    if nota  < menor:
       menor = nota
    
print("nota media es:",suma/n)
print("nota mas baja es ",menor)
```

```python
=int(input("ingree un numero:"))

for i in range (1,13):
    print(f"{i} x {n} = {i*n}")
```

## toma de desicion if elif
```python
num1=int(input("ingrese primer numero:"))
num2=int(input("ingrese segundo numero:"))
num3=int(input("ingrese tercer numero:"))

if num1 > num2:
    if num1 > num3:
        print("El primer numero es mayor",num1)

elif num2 > num1: 
    if num2 > num3:
        print("El segundo numero es mayor",num2)

else:
    print("El tercero numero es mayor",num3)
```

```python
num1=int(input("ingrese temperatura del agua:"))


if num1 < 0:
        print("El estado de agua es solido",num1)

elif num1 <= 100:
        print("El estado de agua es liquido ",num1)

else:
    print("El estado de agua es gaseoso",num1)
```

```python
año=int(input("ingrese año:"))

if año % 4 == 0: 
        if año % 400 == 0 :
             print("El año es bisiesto:",año)

else:
    print("El año no es bisiesto:",año)
```

## ciclo while 
```python
import random

op = 1
valor = 0
victorias = derrotas = empates = 0; 

while op != 0:
    print('<1> Jugar')
    print('<2> Resultados')
    print('<0> Salir')

    op = int(input('Ingrese opcion: '))

    if op == 1:

        while valor<1 or valor>3:
            valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
        
        num = random.randint(1, 3)

        if valor == num:
            print('Empate: ', valor, ' vs ', num)
            empates += 1
        elif valor == 1:
            if num == 2:
                print('Pierdo: ', valor, ' vs ', num)
                derrotas += 1
            elif num == 3:
                print('Gano: ', valor, ' vs ', num)
                victorias += 1
        elif valor == 2:
            if num == 1:
                print('Gano: ', valor, ' vs ', num)
                victorias += 1
            elif num == 3:
                print('Pierdo: ', valor, ' vs ', num)
                derrotas += 1
        elif valor == 3:
            if num == 1:
                print('Pierdo: ', valor, ' vs ', num)
                derrotas += 1
            elif num == 2:
                print('Gano: ', valor, ' vs ', num)
                victorias += 1
    elif op == 2:
        print('Empates:', empates)
        print('Victorias:', victorias)
        print('Derrotas:', derrotas)
        


        # while valor != 1 and valor!=2 and valor!=3:
        #     valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
        
        # while not(valor == 1 or valor == 2 or valor == 3):
        #     valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
        
        # while not(valor>=1 and valor<=3):
        #     valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
```

```python

op = 1
valor = 0
victorias = derrotas = empates = 0;

# 1 si gana el jugador
# 2 si gana la maquina
# 0 empate
def verificar_resultado(jugador, maquina):
    if jugador == maquina:
        return 0
    elif jugador == 1:
        if maquina == 2:
            return 2
        elif maquina == 3:
            return 1
    elif jugador == 2:
        if maquina == 1:
            return 1
        elif maquina == 3:
            return 2
    elif jugador == 3:
        if maquina == 1:
            return 2
        elif maquina == 2:
            return 1

# 1. piedra, 2. papel, 3. tijera
# print(verificar_resultado(3,3))
# print(verificar_resultado(1,2))
# print(verificar_resultado(1,3))

while op != 0:
    print('<1> Jugar')
    print('<2> Resultados')
    print('<0> Salir')

    op = int(input('Ingrese opcion: '))

    if op == 1:

        while valor<1 or valor>3:
            valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
        
        num = random.randint(1, 3)

        resultado = verificar_resultado(valor, num)
        if resultado == 0:
            empates += 1
        elif resultado == 1:
            victorias += 1
        else:
            derrotas += 1


        
    elif op == 2:
        print('Empates:', empates)
        print('Victorias:', victorias)
        print('Derrotas:', derrotas)

    valor = 0
        


        # while valor != 1 and valor!=2 and valor!=3:
        #     valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
        
        # while not(valor == 1 or valor == 2 or valor == 3):
        #     valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
        
        # while not(valor>=1 and valor<=3):
        #     valor = int(input('Ingrese valor: 1. piedra, 2. papel, 3. tijera: '))
```

```python
print ("Introduzca la nota de un estudiante (-1 para salir): ")
grado = int(input())
while grado != -1:
    total = total + grado
    contar = contar + 1
    print ("Introduzca la nota de un estudiante (-1 para salir): ")
    grado = int(input())
promedio = total / contar
print ("Promedio de notas del grado escolar es: " + str(promedio))
```
