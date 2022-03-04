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
