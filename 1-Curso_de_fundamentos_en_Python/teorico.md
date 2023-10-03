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


