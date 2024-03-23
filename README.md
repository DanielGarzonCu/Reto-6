# Reto-6

# PYTHON F.C
 [![PYTHON-F-C-B.jpg](https://i.postimg.cc/1Xpw71f0/PYTHON-F-C-B.jpg)](https://postimg.cc/jnSDC96C)

 # 1 
 Dado la figura de la imagen, desarrolle:
 
 [![image.png](https://i.postimg.cc/664QqD8h/image.png)](https://postimg.cc/pyxv1cY9)
 
 - Una función matemática para calcular el volumen y el área superficial.
 - Cree dos funciones en python para calcular los valores antes establecidos, al ingresar por teclado r1, r2 y h.
 - Revise como utilizar el valor de pi usando import math y math.pi

```ruby
import math

def calcular_volumen(r1, r2, h):
    return (math.pi * (r1**2) * h / 3) + ((r2 ** 3) * 3/4 * math.pi)

def calcular_area_superficial(r1, r2, h):
    return 4 * math.pi * (r2 ** 2) + math.pi * (r1 ** 2) + math.pi * r1 * math.sqrt (h * h + r1 * r2)


r2 = float(input("Ingrese el valor del radio de la esfera: "))
r1 = float(input("Ingrese el valor del radio del cono: "))
h = float(input("Ingrese el valor de la altura del cono: "))


volumen = calcular_volumen(r1, r2, h)
area_superficial = calcular_area_superficial(r1, r2, h)


print(f"El volumen de la figura es: {volumen:.2f}")
print(f"El área superficial de la figura es: {area_superficial:.2f}")
```

# 2 
Dado la figura de la imagen, desarrolle:
[![image.png](https://i.postimg.cc/TY41Pf9Q/image.png)](https://postimg.cc/fJYD2410)

- Una función matemática para calcular el área y el perimetro.
- Cree dos funciones en python para calcular los valores antes establecidos, al ingresar por teclado r, a y b.
- Revise como utilizar el valor de pi usando import math y math.pi

```ruby
import math

def calcular_perimetro(r, a, b):
    return a + b + 2 * (math.pi * r * 2)

def calcular_area(r, a, b):
    return (a * b) + 2 * (math.pi * r ** 2)

if __name__ == "__main__":
    a = float(input("Ingrese el valor de un lado del rectangulo: "))
    b = float(input("Ingrese el valor de otro lado del rectangulo: "))
    r = float(input("Ingrese el valor del radio de los circulos: "))

    perimetro = calcular_perimetro(r, a, b)
    area = calcular_area(r, a, b)

    print(f"El perimetro de la figura es: {perimetro :.2f}")
    print(f"El área de la figura es: {area :.2f}")
```

# 3
Diseñe una función que calcule la cantidad de carne de aves en kilos si se tienen N gallinas, M gallos y K pollitos cada uno pesando 6 kilos, 7 kilos y 1 kilo respectivamente.
```ruby
def calcular_cantidad_carne(F, M, K):

    peso_gallina = 6  
    peso_gallo = 7  
    peso_pollito = 1  

    cantidad_carne_gallina = F * peso_gallina

    cantidad_carne_gallo = M * peso_gallo

    cantidad_carne_pollito = K * peso_pollito

    total_carne = cantidad_carne_gallina + cantidad_carne_gallo + cantidad_carne_pollito

    return total_carne

if __name__ == "__main__":
    
    F = int(input("Ingrese el número de gallinas: "))
    M = int(input("Ingrese el número de gallos: "))
    K = int(input("Ingrese el número de pollitos: "))

    total_carne = calcular_cantidad_carne(F, M, K)

    print(f"La cantidad de carne en en kilogramos es: {total_carne:.2f}")
```

# 4
Mi mamá me manda a comprar P panes a 300 cada uno, M bolsas de leche a 3300 cada una y H huevos a 350 cada uno. Hacer un programa que me diga las vueltas (o lo que quedo debiendo) cuando me da un billete de B pesos.

```ruby
def calcular_cambio(P, M, H, B):

    precio_pan = 3300
    precio_huevo = 350 
    precio_leche = 3300
   
    total = precio_pan * P + precio_leche * M + precio_huevo * H
    return B - total

if __name__ == "__main__":

    P = int(input("Ingrese el número de panes: "))
    M = int(input("Ingrese el número de bolsas de leche: "))
    H = int(input("Ingrese el número de huevos: "))
    B = int(input("Ingrese el valor del billete en pesitos colombianos: "))

    cambio = calcular_cambio(P, M, H, B)

    print(f"El cambio es: {cambio:.2f} pesitos colombianos.")
```

# 5
Haga un programa que utilice una función para calcular el valor de un préstamo C usando interés compuesto del i por n meses.

```ruby
def calcular_valor_prestamo(C, i, n):
 
    return C * (1 + i/n) ** (n*t)

if __name__ == "__main__":

    C = float(input("Ingrese el monto del préstamo: "))
    i = float(input("Ingrese la tasa de interés anual: "))
    n = int(input("Ingrese la cantidad de veces que el interés se compone al año: "))

    # La cantidad de veces que un préstamo se compone al año se refiere a la frecuencia con la que los intereses se calculan y se añaden al capital prestado para determinar el monto total a pagar en cada período de tiempo. #
 
    t = float(input("Ingrese el número de años del préstamo: "))
    V = calcular_valor_prestamo(C, i, n)

    print(f"El valor del préstamo es: {V:.2f} pesos (que dolor).")
```

# 6
El número de contagiados de Covid-19 en el país de NuncaLandia se duplica cada día. Hacer un programa que diga el número total de personas que se han contagiado cuando pasen D días a partir de hoy, si el número de contagiados actuales es C.

```ruby
def calcular_contagiados(C, D):
  
    dias_faltantes = D - 1
    potencia = 2 ** dias_faltantes
    total_contagiados = C * potencia

    return total_contagiados

if __name__ == "__main__":
    
    C = int(input("Ingresa el número de contagiados actuales de Covid-19 en NuncaLandia: "))
    D = int(input("Ingresa el número de días para predecir el número de contagiados: "))

    total_contagiados = calcular_contagiados(C, D)

    print (f"El número total de contagiados después de {D} días será {total_contagiados}")
```

# 7
Escriba un programa que pida 5 números reales y calcule las siguientes operaciones usando una función para cada una:

- El promedio
- La mediana
- El promedio multiplicativo (multilplica todos y luego calcula la raíz de la cantidad de operandos)
- Ordenar los números de forma ascendente
- Ordenar los números de forma descendente
- La potencia del mayor número elevado al menor número
- La raíz cúbica del menor número

```ruby
def calcular_promedio(a, b, c, d, e):
    return (a + b + c + d + e) / 5

def calcular_mediana(a, b, c, d, e):
    numeros_ordenados = sorted([a, b, c, d, e])
    n = len(numeros_ordenados)
    if n % 2 == 0:
        return (numeros_ordenados[n//2 - 1] + numeros_ordenados[n//2]) / 2
    else:
        return numeros_ordenados[n//2]

def calcular_promedio_multiplicativo(a, b, c, d, e):
    producto = a * b * c * d * e
    return producto**(1/5)

def ordenar_ascendentemente(a, b, c, d, e):
    return sorted([a, b, c, d, e])

def ordenar_descendentemente(a, b, c, d, e):
    return sorted([a, b, c, d, e], reverse=True)

def calcular_potencia_mayor_menor(a, b, c, d, e):
    numeros_ordenados = sorted([a, b, c, d, e])
    return numeros_ordenados[-1] ** numeros_ordenados[0]

def calcular_raiz_cubica_menor(a, b, c, d, e):
    numeros_ordenados = sorted([a, b, c, d, e])
    return numeros_ordenados[0] ** (1/3)

if __name__ == "__main__":

    a = float(input("Ingrese un numero: "))
    b = float(input("Ingrese otro numero: "))
    c = float(input("Ingrese otro numero: "))
    d = float(input("Ingrese otro numero: "))
    e = float(input("Ingrese otro numero: "))

    print(f"Promedio: {calcular_promedio(a, b, c, d, e)}")
    print(f"Mediana: {calcular_mediana(a, b, c, d, e)}")
    print(f"Promedio multiplicativo: {calcular_promedio_multiplicativo(a, b, c, d, e)}")
    print(f"Orden ascendente: {ordenar_ascendentemente(a, b, c, d, e)}")
    print(f"Orden descendente: {ordenar_descendentemente(a, b, c, d, e)}")
    print(f"Potencia mayor^menor: {calcular_potencia_mayor_menor(a, b, c, d, e)}")
    print(f"Raíz cúbica del menor número: {calcular_raiz_cubica_menor(a, b, c, d, e)}")
```

# 8
Para el punto anterior incluir las funciones en un archivo independiente e importarlas para su uso.

```ruby
import funciones

if __name__ == "__main__": 
    n1 = float(input("Ingrese el primer número: "))
    n2 = float(input("Ingrese el segundo número: "))
    n3 = float(input("Ingrese el tercer número: "))
    n4 = float(input("Ingrese el cuarto número: "))
    n5 = float(input("Ingrese el quinto número: "))
    print("Sus números son: ",n1,n2,n3,n4,n5)

    n1, n2, n3, n4, n5 = funciones.ordernar(n1,n2,n3,n4,n5)

    promedioNumeros = funciones.promedio(n1,n2,n3,n4,n5)
    
    medianaNumeros = funciones.mediana(n1,n2,n3,n4,n5)

    promedioMultiNumeros = funciones.promedio_multiplicativo(n1,n2,n3,n4,n5)

    ascendenteNumeros = funciones.ascendente(n1,n2,n3,n4,n5)

    descendenteNumeros = funciones.descendente(n1,n2,n3,n4,n5)

    potenciaNumeros = funciones.potencia(n1,n2,n3,n4,n5)

    raizNumeros = funciones.raiz(n1,n2,n3,n4,n5) 

    print("El promedio de los números es: ", promedioNumeros)
    print("La mediana de los números es: ", medianaNumeros)
    print("El promedio multiplicativo de los números es: ", promedioMultiNumeros)
    print("El orden ascendente de los números es: ", ascendenteNumeros)
    print("El orden descendente de los números es: ", descendenteNumeros)
    print("La potencia del mayor elevado al menor es ", potenciaNumeros)
    print("La raiz cubica del menor es ", raizNumeros)

```

# 9
Consultar qué es y cómo funciona pip en python.

<details>
  <summary>¿pip?</summary>
  
  Pip es como el 'app store' de Python. Te permite descargar y administrar todas esas 'apps' o paquetes de Python que la gente ha creado y comparte en internet. Imagínalo como tu asistente personal que te ayuda 
 a encontrar, instalar y actualizar todas esas herramientas geniales que otros programadores han hecho.
 Cuando necesitas una nueva función en tu proyecto de Python, simplemente le dices a pip qué paquete necesitas y él se encarga de todo el proceso de instalación. Y si alguna vez necesitas actualizar un paquete 
 para obtener las últimas funciones, pip también puede hacer eso con un simple comando.
 Además, si ya no necesitas un paquete, pip puede eliminarlo fácilmente de tu sistema. También puede manejar la instalación de todos los paquetes necesarios para un proyecto a partir de un archivo de requisitos, 
 lo que hace que sea muy sencillo compartir y colaborar en proyectos con otros programadores.
 
</details>

# 10 
Hacer un listado de módulos populares para python que se puedan instalar com pip y consultar cómo instalarlos.

<details>
  <summary>10 Modulos populares</summary>
  Para instalar cualquiera de estos módulos, simplemente ejecuta el comando de instalación correspondiente utilizando pip en tu terminal o símbolo del sistema. 
  numpy: Para computación numérica eficiente en Python.
Instalación: pip install numpy

pandas: Para manipulación y análisis de datos estructurados.
Instalación: pip install pandas

matplotlib: Para trazar gráficos y visualizar datos de manera efectiva.
Instalación: pip install matplotlib

scikit-learn: Para aprendizaje automático y minería de datos.
Instalación: pip install scikit-learn

tensorflow: Para construir y entrenar modelos de aprendizaje profundo.
Instalación: pip install tensorflow

PyTorch: Otro marco popular para el aprendizaje profundo.
Instalación: pip install torch

Django: Para desarrollo web rápido y flexible en Python.
Instalación: pip install django

Flask: Un micro marco de desarrollo web para Python.
Instalación: pip install flask

requests: Para hacer solicitudes HTTP en Python de manera sencilla.
Instalación: pip install requests

beautifulsoup4: Para extraer datos de HTML y XML.
Instalación: pip install beautifulsoup4

</details>

