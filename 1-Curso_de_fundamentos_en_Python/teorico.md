# Curso de fundamentos en Python

Python se ha convertido en uno de los lenguajes de programación más populares del mundo en los últimos años. Se utiliza en todo, desde el aprendizaje automático hasta la construcción de sitios web, y se utiliza por desarrolladores como no desarrolladores.

## Que es identacion?
Se refiere que se debe respetar la sangria en estado 0 de cada linea de codigo.

        IndentationError: unexpected indent
        exit status 1
         ^C
        

## Comando para imprimir print("contenido")

        print("hola mundo")
        print("hola soy jose y este es mi mundo")
        print(12+2)

## Comentarios # y tambien """ triple comilla 

        # Comentario simple 
        
        """ Comentario grande
        print("hola mundo")
        print("hola soy jose y este es mi mundo")
        print(12+2)        
        """
## Variables 

Primeramente para ejecutar otro archivo que queramos, tendremos que dirigirnos al la shell y tendremos que escribir:

        python archivo.py

vars.py 

        print("Estamos en vars")

        my_name = "jose"
        my_age = 27

        print(my_name)
        print(my_age)
        print("Mi nombre es ", my_name, "y tengo", my_age, "añós")  #concatenado

* Input: Valor para mandar por consola 

        my_name = input("Cual es tu nombre?")
        print("Tu nombre es", my_name)

* Calculadora de 2 variables
            
        a = int(input("introduce un numero: "))
        b = int(input("introduce otro numero: "))

        suma = a + b
        print("la suma es", suma)


## Tipos de datos primitivos
* Integers: números Enteros 
        
        #Int
        my_age = 12
        print("el valor", my_age, "es de", type(my_age))

* Floats: números de punto flotante (decimales)

        #Float
        temperature = 12.12
        print("el valor", temperature, "es de", type(temperature))

* Strings: cadena de caracteres (texto)

        #Strings
        my_name = "jose"
        my_name = 'jose'
        print("el valor", my_name, "es de", type(my_name))

* Boolean: boolenaos (Verdadero o Falso)

        #Boolean
        is_single = False
        print("el valor", is_single, "es de", type(is_single))

### Tipos de dato adicionales
* Datos en texto: str
* Datos numéricos: int, float, complex
* Datos en secuencia: list, tuple, range
* Datos de mapeo: dict
* Set Types: set, frozenset
* Datos booleanos: bool
* Datos binarios: bytes, bytearray, memoryview

* Inputs

        #Inputs vamos a determinar que tipo es introduciendo un valor

        valor = input("Introduce un valor y te dire de que tipo es:")
        print("el valor", valor, "que introduciste es de", type(valor))

* Concatenacion 
  
        # Concatenar
        name = "Jose"
        last_name = "Pabon"
        full_name = "Nombre completo: " + name + " " + last_name
        print(full_name)

        # Cuando queramos utilizar comillas para strings debemos intercalar ejemplo:

            oracion = "i'm jose"
            oracion2 = 'she said "hello jose"'

* Maneras de imprimir datos 

        name = "Jose"
        last_name = "Pabon"

        #formatos

        format_1 = "Hola mi nombre es " + name + " y mi apellido es " + last_name
        print("v1", format_1)

        format_2 = "Hola mi nombre es {} y mi apellido es {}".format(name, last_name)
        print("v2", format_2)

***No te olvides la f de format***

        format_3 = f"Hola mi nombre es {name} y mi apellido es {last_name}"
        print("v3", format_3)

 ## Trasformaciones de tipo 
 * str nos permite convertir una cadena a numero

        name = "jose"
        str(name) = 4 

## Operadores aritmeticos

        print(10 + 10)  #Operador de suma
        print(10 - 10)  #Operador de resta
        print(10 * 10)  #Operador de multiplicasion
        print(10 / 10)  #Operador de division
        print(10 % 10)  #Operador de modulo osea residuo
        print(
        10 % 10
        )  #Operador de division enterea osea que nos quedamos con el valor entero de la division
        print(10**10)  #Operador de exponensiacion

* Orden de ejecucion

        # Orden de ejecucion
        # P parentesis
        # E exponentes
        # M multiplicacion
        # D Division
        # A Adicion
        # S Sustraccion
* OJO no se puede dividir entre 0 python te lanza error

## Operadores de comparacion 
* Comparacion 

        # > Mayor que

        print(2 > 5)

        # < Menor que

        print(2 < 5)

        # >= Mayor igual que

        print(2 >= 5)

        # <= Menor igual que

        print(2 <= 5)

* Igualacion 

        # Igual netamente iguales
        print(5==5)# 5 es igual a 5 ?
        print(5==4)

        # Diferente 
        print(5 != 5)# 5 es diferente que 5 ?
        print(5 != 4)

## Comparacion de numeros flotantes

* Existen siertos problemas para comparar numeros flotantes ya que algunos cuentan con una precision diferente 
        
        #Por ejemplo  
        x = 3.3
        y = 1.1 + 2.2
        print(x) # Nos da 3.3
        print(y) # Nos da 3.3000000001
        Al momento de comparar nos saldra Falso
        print(x==y) 

* Como podemos cortar esa precision?

        y_str = format(y,".2g") # Le aplicamos formato para tener 2g digitos nada mas
        print(x==y_str) #Nos dara true

* Forma matematica 
        
        x = 3.3
        y = 1.1 + 2.2
        #Creamos una tolerancia 
        tolerancia = 0.00001

        print(abs(x-y)<tolerancia)

## Operadores logicos 
### AND

        #AND si ambas condiciones son verdaderas da TRUE

                1 and 1 = TRUE
                0 and 1 = FALSE
                1 and 0 = FALSE
                0 and 0 = FALSE

        print (5 > 4 and 4>3)

* Ejemplo practico
        
        #El valor que debemos introducir debe ser >=100 y <=1000 solo asi recibiremos un TRUE
        stock = input("ingrese un numero para el stock:")
        stock = int(stock)
        print (stock>=100 and stock <=1000)

### OR

        # OR si una de las variables es true nos resulta TRUE
                1 or 1 = TRUE
                0 or 1 = TRUE
                1 or 0 = TRUE
                0 or 0 = FALSE
### NOT

       # Revierte el valor de cualquier ya antes mencionado

## Condicionales

        # IF
        animal = input('Cual es tu animal favorito:')
        if animal == 'perro':
        print("los perros son los mejores amigos del hombre")
        if animal == 'gato':
        print("los gatos son muy independientes")
        if animal == 'leon':
        print("El leon es el rey de la selva")
        if animal == 'tigre':
        print("El tigre siempre segundo")
        else:
        print("lo siento tu animal no existe en la database")

        # ELIF es lo mismo
         animal = input('Cual es tu animal favorito:')
        if animal == 'perro':
        print("los perros son los mejores amigos del hombre")
        elif animal == 'gato':
        print("los gatos son muy independientes")
        else: 
        print("lo siento tu animal no existe en la database")

* Reto de numeros impares 

        numbre = int(input('Ingrese algun valor:'));
        result= number % 2 
        if (result=0):
                print('Es par')
        else:        
                print(  'Es impar')

## Proyecto condicionales 

        # Juego de piedra papel o tijera

## Funciones para STINGS

* in nos permite saber si existe un valor dentro de un texto o campo

        text = "Ella sapeeee programar en Pythin"# Funcion in 'variable o tambien puede ser array'
        
        print('en' in text)
        if ("Ella" in text):
        print('Si existe pero ella no te ama')
        elif ('sapeeee' in text):
        print('Nop')
        else:
        print('nop')

*  len Nos permite contar cuantos caracteres hay en un array # o texto, ojo cuenta los espacios

        size = len('El jose sapeeee')
        print(size)
        text = "Ella sapeeee programar en Pythin"
        print(text.upper())  #MAYUSCULAS
        print(text.lower())  #minusculas
        print(text.count('a'))  #Cuenta las a's del texto
        print(text.swapcase())  #Revierte los caracteres del texto may a min
        print(text.startswith('Ella'))  # Preguntamos si el texto #empieza con ella
        print(text.endswith('e'))  # Termina en e?

* Reemplazar

        print(text.replace('Pythin','Python'))  #Le decimos que reemplase Pythin por Python


* Pregunta si es digito 

        print('114'.isdigit()) #Debe responder TRUE
### Mas metodos

1. capitaliza      Cambia todas las letras a minúsculas menos la primera.
2. casefold        Utilizada para compara cadenas sin importar el tamaño de los caracteres.
3.  center          Formaseta una cadena alineandola al centro
4.  count           Cuenta las ocurrencias de una cadena
5.  encode          Codifica una cadena según la codificación deseada.
6.  endswith        Comprueba si la cadena termina con una cadena específica.
7.  expandtabs      Convierte los tabuladores en espacios.
8.  find            Devuelve el índice de la cadena buscada o -1 si no se encuentra.
9.  format          Formatea una cadena de forma avanzada.
10. format_map      Igual que format, pero sin hacer una copia de los parámetros.
11. index           Devuelve el índice de una cadena de caracteres o ValueError.
12. isalnum         Comprueba si la cadena es alfanumérica.
13. isalpha         Comprueba si la cadena es alfabética.
14. isascci         Comprueba si la cadena es ASCII.
15. isdecimal       Comprueba si la cadena es un decimal.
16. isdigit         Comprueba si la cadena es un dígito.
17. isidentifier    Comprueba si la cadena es un identificador.
18. islower         Comprueba si todos los caracteres son minúsculos.
19. isnumeric       Comprueba si la cadena es numérica.
20. isprintable     Comprueba si la cadena es imprimible.
21. isspace         Comprueba si la cadena solo contiene espacios.
22. istitle         Comprueba si la cadena tiene formato de título.
23. isupper         Comprueba si todos los caracteres son mayúsculas.
24. join            Une todos los elementos de un iterador en una cadena.
25. ljust           Justifica la cadena a la izquierda.
26. lower           Convierte la cadena a minúsculas.
27. lstrip          Elimina los caracteres de espacio de la izquierda.
28. maketrans       Crea una tabla de traducción para translate.
29. partition       Crea particiones de una cadena usando un separador.
30. replace         Reemplaza en la misma cadena un carácter por otro.
31. removeprefix    Devuelve una nueva cadena con el prefijo especificado como argumento eliminado si se encuentra en la cadena origina.
32. removesuffix    Devuelve una nueva cadena con el sufijo especificado
33. rfin            Devuelve el índice de la cadena como parámetro buscando por la derecha o -1 si no se encuentra.
34. rindex          Devuelve el índice de la cadena como parámetro buscando por la derecha o ValueError.
35. rjust           Justifica la cadena a la derecha.
36. rpartition      Crea particiones de una cadena usando un separador y comenzando por la derecha.
37. rsplit          Devuelve una lista de cadenas al separar la original por un separador buscando por la derecha.
38. rstrip          Devuelve una lista de cadenas separando la original por saltos de línea.
39. split           Devuelve una lista de cadenas al separar la original por un separador.
40. splitlines      Devuelve una lista de cadenas separando la original por saltos de línea.
41. startswith      Comprueba si la cadena comienza con una cadena específica.
42. strip           Elimina los espacios iniciales y finales de la cadena.
43. swapcase        Cambia el tamaño de cada letra de minúsculas a Mayúsculas y las que estan en Mayúsculas a minúsculas.
44. title           Convierte la cadena a formato título.
45. translate       Reemplaza cada carácter por otro siguiendo una tabla de traducciones.
46. upper           Convierte la cadena a mayúsculas.
47. zfill           Añade ceros a la izquierda a una cadena numérica.

## Indexin y slicing 
### Indexin 
* Son como arrays

        text = "Ella sapeeee programar en Pythin"
        #Quiero saber cual es el caracter segun el orden que defino #empiezan desde 0
        print(text[0])  #Imprimira E
        print(text[5])  #Imprimira s

* Como saber cual es el ultimo valor del texto
        
        print(text[len(text) - 1])  #Mas usada haha

###  Silicing
* Se refiere a que podemos colocar 2 valores uno para indicar en que caracter comenzar y otro para terminar
       
        text = "Ella sapeeee programar en Pythin"
        print(text[0:5])  #Extrae Ella
        print(text[:5])  #Otro tipo de sintaxis
        print(text[5:])  #Inicia desde el caracter 5 hasta el final
        print(text[:])  #Inicia en 0 y termina en el final
        print(text[:-1])  #Nos lleva al final menos 1

* Saltos

        print(text[12:22:1]) # Saltara valores de uno en uno en el #rango especificado
        print(text[12:22:3]) # Saltara valores de uno en uno en el #rango especificado



## Listas

        numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
        print(numbers[0])

        strings = ['uno', 'dos', 'tres', 'cuatro', 'cinco']
        print(strings)

        types = ['uno', 2, 'tres', 4, 'cinco']
        print(type(types))
        types[0]= 1 # reemplaza el valor string por un number
        print(types[:])


* Puede ser modificada
* Cada elemento esta separado por una coma
* Puede contener todo tipo de datos
* Metodos para listas
* Lista.metodo(indice,elemento) o Lista.metodo(elemento)

### Metodos importantes

* count(elemento) cuenta cuantas veces un elemento esta en una lista

* extend(lista) permite extender una lista agregándole los elementos de otra lista

* pop() elimina y retorna el ultimo elemento de la lista

* reverse() reversa el orden de la lista

* sort() ordena la lista de manera ascendente o descendente

### Actualizar un valor

        Lista = [1, 2, 3, 4, 5]

        Lista[0] = -8

        Lista = [-8, 2, 3, 4, 5], resultado de la lista luego de actualizar el valor

        Agregar un elemento

        Lista.append(indice,elemento) o

        Lista.append(elemento) en este caso el nuevo elemento se agrega al final de la lista

        Eliminar un elemento

        Lista.remove(indice, elemento)

## Métodos de las listas

        lista.metodo(posicion)
        numeros.pop(5)

* append(): Añade un ítem al final de la lista.
* clear(): Vacía todos los ítems de una lista.
* extend(): Une una lista a otra.
* count(): Cuenta el número de veces que aparece un ítem.
* index(): Devuelve el índice en el que aparece un ítem (error si no aparece).
* insert(): Agrega un ítem a la lista en un índice específico.
* pop(): Extrae un ítem de la lista y lo borra.
* remove(): Borra el primer ítem de la lista cuyo valor concuerde con el que indicamos.
* reverse(): Le da la vuelta a la lista actual.
* sort(): Ordena automáticamente los ítems de una lista por su valor de menor a mayor.

###  Otra forma de seleccionar el ultimo valor de la lista
        numbers = [1, 2, 3, 4, 5]
        numbers[-1] = 10
        print(numbers[-1])  #
        #* append se lo utiliza para agregar un valor x al final de una lista
        numbers.append(-9)
        print(numbers)
        #insert inserta datos en la posision que seleccionamos
        numbers.insert(0, 'el 1 fue reemplazado')
        print(numbers)

### FUSIONAR LISTAS
        Personas = ['jose', 'ramiro', 'sebas']
        Tareas = ['tarea_1', 'tarea_2', 'tarea_3', 'tarea_4']
        new_list = Personas + Tareas
        print(new_list)

### Consultar si un elemento se encuentra dentreo de una lista

        index = new_list.index('tarea_3')
        print(new_list.insert(index, "Tarea terminada"))


## Tuplas
 Estructura de datos inmutables que contiene una secuencia ordenada de elementos

        Tupla = (1, 2, 3, 4)

- Los elementos están separados por espacios luego de las comas
- Puede contener cualquier tipo de datos
- Cada posición de la tupla tiene un índice
- Es inmutable y por lo tanto no puede ser modificada, lo que permite proteger mejor la data si no queremos que se modifique por error 

* Acceder a un elemento
        
        Tupla = (”A”, “B”, “C”)
        Tupla [0] Indice a consultar

        # “A” Nos retorna el resultado de la posición 0 en la tupla

* Encontrar un elemento
        
        Tupla = (”A”, “B”, “C”)

        “A” in Tupla

        True

        “Z” in Tupla

        False

### Metodos en tuplas

* Buscar el Indice de un elemento

        Tupla = (”A”, “B”, “C”)

        Tupla.index(”A”)

        0 Nos devuelve el indice del elemento que buscamos

* Numero de veces que un elemento aparece en la Tupla

        Tupla = (”A”, “B”, “C”)

        Tupla.count(elemento)

        Tupla.count(”B”)

        # 1 Retorna el numero de veces del elemento en la Tupla

* Trasformar una tupla a lista 

        Tupla = (”A”, “B”, “C”)
        lista = list(Tupla)

* Trasformar una lista a tupla 

        Lista = (”A”, “B”, “C”)
        Tupla = tuple(Lista)

### Piedra papel o tijera con tuplas

        import random # importamos la libreria random

        options = (“piedra”, “papel”,“tijera”)# tupla para la seleccion de la maquina
        
        computer_option = random.choice(options)# la computadora elige un valor aleatoreo 
        
        user_option= 1
        while user_option not in options:
        user_option = input("piedra, papel o tijera: ").lower()

        if user_option == computer_option:
        print(“Empate!”)
        elif user_option == “piedra”:
        if computer_option == “tijera”:
        print(“piedra gana a tijera”)
        print(“user gano!”)
        else:
        print(“Papel gana a piedra”)
        print(“computer gano!”)
        elif user_option == “papel” :
        if computer_option == “piedra”:
        print(“papel gana a piedra”)
        print(“user gano!”)
        else:
        print(“tijera gana a papel”)
        print(“computer gano!”)
        else: # user tiene tijera
        if computer_option == “papel”:
        print(“tijera gana a papel”)
        print(“user gano!”)
        else:
        print(“piedra gana a tijera”)
        print(“computer gano!”)

## Diccionarios  
* Los diccionarios se compones de llave, valor. muy similares a un archivo .json

        my_dictionary = {
        'avion': 'objeto volador',
        'name': 'Javier',
        'last_name': 'Sepulveda',
        'age': 109
        }

        print(my_dictionary)

        #el tamanio del diccionario
        print(len(my_dictionary))

        #imprimiendo una llave 
        print(my_dictionary['age'])

* La funcion get, si no existe el valor sale un mensaje none(Maneja el error)
* Se cambian los corchetes por parentesis(), ya que get es una funcion de python print(my_dict.get('test'))

        print('name' in my_dictionary)
        print('other' in my_dictionary)

## Metodos CRUD para los diccionarios

        print("--- "*5)
        #Diccionario
        person= {
        'name': 'Camilo',
        'last_name': 'Rico',
        'langs': ['python', 'javascript'],
        'age': 99
        }

        print(person)

        person['name']='Camilo Andres' #Insertar valores
        person['age']-=50 # Le resta a la edad actual los 50 que serian 49
        person['langs'].append('rust') # Introduce el valor rust al final de los atributos
        print(person) 
        del person['last_name']
        person.pop('age') 
        print(person)


        print(person.items()) # Imprime items 
        print(person.keys()) # Imprime las llaves o atributos 
        print(person.values()) # Nos muestra todos los valores
        print(person.clear()) # Limpia el diccionarios


##  Ciclos
### While Mientras
While es un ciclo que se ejecuta mientras la concicion sea verdadera

* Tabla de multiplicar

        i = 0 # Se inicia un contador para aumentar 
        x = (int(input('Numero para la tabla de multiplicar que deceaas: '))) # Seleccionamos un valor repetitivo para la estructura de la tabla
        y = (int(input(f'Hasta que numero quieres multiplicar {x}: '))) # Introducimos las veces que queremos que se repita la condicion

        while i < y: # Esttuctura para que se repita la condicion
        i += 1 # aumenta para que se cumpla la condicion
        print(f'{x} x {i} = {x*i}')

* Arbolito de navidad

        i = 0
        x = int(input('Cuantas filas quieres que tenga tu arbol de navidad? :'))
        while i < x:
          i += 1
          print((' ' * (x - i)) + ('*' * (2 * i - 1)))
## Ciclo FOR

        x = int(input('x:'))
        y = input('y:')
        for x in range(x):
          print(y)

### Recorrer listas
        mi_lista = [12, 14, 23, 45, 56]
        for element in mi_lista:  # Existe un elemento en mi lista
        print(element)  # Imprime la lista

### Recorrer tuplas

        mi_tupla = ('jose', 28, 'pabon', 2023)
        for element in mi_tupla:
        print(element)

### Recorrer Diccionarios
        mi_diccionario = {
        'nombre': 'jose',
        'edad': 28,
        'apellido': 'pabon',
        'anio': 2023
        }
        for element in mi_diccionario:
        print(element, '=', mi_diccionario[element])
        #Lista de diccionarios
        lista_dict = [{
        'nombre': 'jose',
        'edad': 28
        }, {
        'nombre': 'Raul',
        'edad': 38
        }, {
        'nombre': 'Fernando',
        'edad': 78
        }]
        for person in lista_dict:
        print()
# Ciclos anidados

        matriz = [
        [1, 2, 3], 
        [4, 5, 6], 
        [7, 8, 9]
        ]

* Imprime la primera fila de la matriz
        
        print(matriz[0])

* Imprime el elemento 2 de la primera fila
        
        print(matriz[0][1])

Recorremos las filas de la matriz y por cada fila recorremos cada una de las columnas

        for row in matriz:
        print(row)
        for column in row:
        print(column)

## Juego de piedra papel y tijera con todo lo aprendido

        import random 

        options = ('piedra', 'papel', 'tijera')
        rounds = 1
        computer_wins = 0 
        user_wins = 0

        print("""
        [ 🤖 Bienvenido al juego Piedra, Papel o tijera 🙋]
                        >>> Ingresa una opción <<<
        """)

        while True:
        print('***' * 10)
        print('Round ', rounds)
        print('***' * 10)
        
        print(f'''
        🤖 Computer wins: {computer_wins}
        🙋 User wins: {user_wins}
                ''')
        
        user_option = input('>>> Piedra, papel o tijera => ').lower()
        rounds += 1
        
        if not user_option in options:
                print('Esa opción no es valida')
                
        computer_option = random.choice(options)

        print('User option => ', user_option)
        print('Computer option => ', computer_option)

        if user_option == computer_option:
                print('Empate!\n')
        elif user_option == 'piedra':
                if computer_option == 'tijera':
                print('🪨 Piedra gana a tijera ✂️')
                print('¡User gana!\n')
                user_wins += 1
                else:
                print('📄 Papel gana a piedra 🪨')
                print('¡Computer gana!\n')
                computer_wins += 1
        elif user_option == 'papel':
                if computer_option == 'piedra':
                print('📄 Papel gana a piedra 🪨')
                print('¡User gana!\n')
                user_wins += 1
                else:
                print('✂️ Tijera gana a papel 📄')
                print('¡Computer gana!\n')
                computer_wins += 1
        elif user_option == 'tijera':
                if computer_option == 'papel':
                print('✂️ Tijera gana a papel 📄')
                print('¡User gana!\n')
                user_wins += 1
                else:
                print('🪨 Piedra gana a tijera ✂️')
                print('¡Computer gana!\n')
                computer_wins += 1
        
        if computer_wins == 3:
                print('🎖️ El ganador es Computer 🎖️')
                break
        
        if user_wins == 3:
                print('🎖️ El ganador es User 🎖️')
                break