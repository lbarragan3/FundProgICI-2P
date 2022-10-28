# **Ejercicios de Clase**
### **Resolución de problemas de clase con Diagramas de Flujo de Datos**
## **Ejercicio 1.**
#### Contar del 1 al 10 y sumar los valores.
#### 1.1 Análisis
Usar el símbolo de proceso para dar valor a la variable suma, además de realizar un contador donde los números deberan de cumplir con la condición, si estos ecceden las condiciones establecidas imprimir el contador para finalizar.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E1_for](https://user-images.githubusercontent.com/113486125/197885895-9e397154-f881-430b-9ff0-fed40436b163.png)

**_Ciclo while:_**

![E1_while](https://user-images.githubusercontent.com/113486125/197885913-5154a9d2-129b-4e4f-9ab5-33ccc55dab88.png)

**_Ciclo do-while:_**

![E1_dowhile](https://user-images.githubusercontent.com/113486125/197885931-8342307d-d520-4fbb-8d58-e243423fbe9c.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s");
}
```
**_Ciclo while:_**
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
```
**_Ciclo do-while:_**
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s += c;
    c++;
  } while (c <= 10);
  print("El resultado de la suma de los valores es:$s");
```

#### 1.3 Prueba de Escritorio
| Datos | cont<=10 | mensaje | salida |
| ----------- | ----------- | ----------- | ----------- |
| c=1 | si, cont=cont+1 | s | 55 |
| s=0 | no, fin captura |  |  |

#### 1.4 Entradas
Ninguna
#### Salidas
55



## **Ejercicio 2.**
#### Obtener la suma de los primeros 5 números pares
#### 1.1 Análisis
Usar el símbolo de proceso para dar valor a la variable suma, sumar los procesos del contador y verificar que los números cumplan ciertas condiciones.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E2_for](https://user-images.githubusercontent.com/113486125/197885993-9e44bc07-2484-430c-afa0-ba189dd94552.png)

**_Ciclo while:_**

![E2_while](https://user-images.githubusercontent.com/113486125/197886012-102d6ac6-15d9-4816-b94a-3d081dab6234.png)

**_Ciclo do-while:_**

![E2_dowhile](https://user-images.githubusercontent.com/113486125/197886028-490ea975-0f78-4d14-be0c-b38fdd352370.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 2; i <= 10; i = i + 2) {
    s = s + i;
  }
  print("resultado de la suma de numeros pares es:$s");
}
```
**_Ciclo while:_**
```dart
void main(List<String> args) {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
}
```
**_Ciclo do-while:_**
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("la suma de numeros pares es:$s");
}
```

#### 1.4 Entradas
Ninguna
#### Salidas
30


## **Ejercicio 3.**
#### Obtener la suma de los primeros 5 números pares
#### 1.1 Análisis
Almacena en un array el número n liedo del teclado, el tamaño del array es 10.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E3_for](https://user-images.githubusercontent.com/113486125/197886097-c0518a6d-aed3-4493-ba9c-4876f8156e8e.png)

**_Ciclo while:_**

![E3_while](https://user-images.githubusercontent.com/113486125/197886111-0e614e32-9983-45cf-9ca9-d571337454d8.png)

**_Ciclo do-while:_**

![E3_dowhile](https://user-images.githubusercontent.com/113486125/197886128-c38851a5-7071-441c-9b5e-0e800f1be151.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
**_Ciclo while:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
**_Ciclo do-while:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```

#### 1.4 Entradas
Ninguna
#### Salidas
30


## **Ejercicio 4.**
#### Almacene los n números leidos del teclado en un vector de 10 elementos.
#### 1.1 Análisis
Usar el símbolo de proceso para crear un array para los 10 elementos donde se almacenaran los números leidos del teclado, posteriormente verificar que cada número entre en el arreglo y almacenarlo hasta que se llenen los 10 elementos del array.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E4_for](https://user-images.githubusercontent.com/113486125/197888615-d09de661-8784-4797-a497-34b2f80c0870.png)

**_Ciclo while:_**

![E4_while](https://user-images.githubusercontent.com/113486125/197888630-554dcfea-1678-4e6f-83ce-5046b2681776.png)

**_Ciclo do-while:_**

![E4_dowhile](https://user-images.githubusercontent.com/113486125/197888655-90794ce0-6a1d-485f-96e5-62b229a24b4a.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
**_Ciclo while:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
**_Ciclo do-while:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```

#### 1.4 Entradas
10 números leídos del teclado.
#### Salidas
A[10], lleno con elementos


## **Ejercicio 5.**
#### Almacene un contador negativo en un vector, el conteo es de 10 a 0.
#### 1.1 Análisis
En el símbolo de proceso asignar un array de 11 elementos y el contador, verificar que desde el principio el primero número sea 10 y que este haga una cuenta regresiva desde ese número hasta 0.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E5_for](https://user-images.githubusercontent.com/113486125/197889524-7c47b651-80df-4198-943c-66f4b9563346.png)

**_Ciclo while:_**

![E5_while](https://user-images.githubusercontent.com/113486125/197889537-783bd811-68cc-4303-96e5-701cf4bee076.png)

**_Ciclo do-while:_**

![E5_dowhile](https://user-images.githubusercontent.com/113486125/197889560-a9362529-a358-431b-971f-9942cd6a5abc.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}
```
**_Ciclo while:_**
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  while (c >= 0) {
    arr[10 - c] = c;
    c = c - 1;
  }
  print(arr);
}
```
**_Ciclo do-while:_**
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  do {
    arr[10 - c] = c;
    c = c - 1;
  } while (c >= 0);
  print(arr);
}
```

#### 1.4 Entradas
Ninguna
#### Salidas
A[10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]


## **Ejercicio 6.**
#### Almacene en un vector de tamaño 10, todos los números pares capturados hasta completar todos.
#### 1.1 Análisis
Usar el símbolo de proceso para asignar un array de 10 elementos, un contador y una suma para contdor, usar el símbolo de entrada de datos para que el usuario ingrese los números, verificar que cada número ingresado sea par y almacenar en el array, hacer este proceso hasta que se llenen los 10 elementos del vector.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E6_for](https://user-images.githubusercontent.com/113486125/197890670-3f4f651e-3ee6-4297-9317-7729f91ff750.png)

**_Ciclo while:_**

![E6_while](https://user-images.githubusercontent.com/113486125/197890680-b4257a76-2eeb-47e8-8815-7c94a8c02413.png)

**_Ciclo do-while:_**

![E6_dowhile](https://user-images.githubusercontent.com/113486125/197890690-4e9ab3d0-c4d7-4f5e-a4d9-a33a352aed1b.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```python
numeros = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]



def extraer_pares(lista):
    pares = []

    for n in lista:
        if n % 2 == 0:
            pares.append(n)

    return pares

print()

resultado = extraer_pares(numeros)

print("Contenido de la variable`resultado`:", resultado)
print("Cantidad de elementos en la lista `resultado`:", len(resultado))
```
**_Ciclo while:_**
```python
numeros = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]

print("Contenido de la variable`numeros`:", numeros)
print("Cantidad de elementos en la lista `numeros`:", len(numeros))

def extraer_pares(lista):
    pares = []

    while(true):
        if n % 2 == 0:
            pares.append(n)

    return pares

print()



print("Contenido de la variable`resultado`:", resultado)
print("Cantidad de elementos en la lista `resultado`:", len(resultado))
```
**_Ciclo do-while:_**
```dart
void main() {
  var array = [];
  var c = 0;
  do {
    int n = int.parse(stdin.readLineSync()!);

    if (n % 2 == 0) {
      array.add(n);
      c = c + 1;
    }
  } while (c <= 9);
  print(array);
}
```

#### 1.4 Entradas
Números ingresados por el usuario
#### Salidas
A[10]= numeros %2 == 0


## **Ejercicio 7.**
#### Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados. La calificación esta entre 0 y 10, y el máximo de alumnos es de 15.
#### 1.1 Análisis
Crear un array de 15 elementos, un contador y una suma para contador con el símbolo de proceso, con el símbolo de entrada de datos el usuario ingresará cada calificación hasta completar los 15 elementos del vector, cada elemento tiene que pasar por el condicional para saber si es mayor-igual a 6 o menor que este, al final se imprimiran las calificaciones, el promedio de las aprobatorias y la cantidad de alumnos reprobados.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E7_for](https://user-images.githubusercontent.com/113486125/197893440-243df8fc-1aa0-42c3-b8ac-daa17f5ea4de.png)

**_Ciclo while:_**

![E7_while](https://user-images.githubusercontent.com/113486125/197893453-2252d574-2253-4724-b92e-92815263fe5a.png)

**_Ciclo do-while:_**

![E7_dowhile](https://user-images.githubusercontent.com/113486125/197893471-250e4d32-5aec-4cdd-bf4f-b790d73acfce.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```python
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
**_Ciclo while:_**
```python
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
**_Ciclo do-while:_**
```dart
void main() {
  double PromA = 0;
  var contr = 0;
  double sumaA = 0;
  double contA = 0;
  double cal1 = 0;
  double cal2 = 1;
  var cont = 0;
  stdout.write("Dame las calificaciones\n ");
  stdout.write("----------\n");
  do {
    double c = double.parse(stdin.readLineSync()!);
    cont = cont +1;
    if (c > 10) {
      print('La calificacion no puede ser mayor a 10');
      cont = cont - 1;
    }
    if (c < 0) {
      print('La calificacion no puede ser menor a 0');
      cont = cont - 1;
    }
    if (c < 6 && c > 0) {
      contr = contr + 1;
    }
    if (c <= 10 && c >= 6) {
      cal1 = c;
      sumaA = sumaA + cal1;
      contA++;
    }
    if (cal1 > cal2) {
      cal2 = cal1;
    }
  } while (cont <= 14);
  PromA = sumaA / contA;
  print('El promedio de aprobados es $PromA');
  print('La calificacion mas alta es $cal2');
  print('La cantidad de reprobados son $contr');
}
```

#### 1.4 Entradas
Calificacines
#### Salidas
Calificaciones, promedio de las calificaciones aprobatorias y cantidad de alumnos reprobados.


## **Ejercicio 8.**
#### Capture n números en el rango [Li,Ls] donde: -Li = Limite inferior -Ls limite superior para li<ls y l0, obtenga: Cantidad de números pares y su promedio, Cantidad de números impares y su promedio y ¿Qué promedio es mayor?
#### 1.1 Análisis
Usar el símbolo de proceso para asignar suma para pares e impares, un contador para pares e impares, y el promedio para pares e impares, pedir al usuario limite inferior y superior, verificar que Li sea mayor a cero y Ls mayor a Li; pedir al usuario que ingrese los números (pedir un límite para que el ciclo no sea infinito). Comprobar cuántos números son pares y cuántos impares, obtener el promedio de los pares y de los impares, comprobar si el promedio de los pares es mayor o el de los impares, imprimir cual es mayor.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E8_for](https://user-images.githubusercontent.com/113486125/198382593-2f8fdfa5-ddd5-47f6-8e37-005659b8dbc3.png)

**_Ciclo while:_**

![E8_while](https://user-images.githubusercontent.com/113486125/198385225-d38f30fe-9ac7-4f07-9a1a-6b94a49904e2.png)

**_Ciclo do-while:_**

![E8_dowhile](https://user-images.githubusercontent.com/113486125/198385245-29ab15f4-210e-495e-8269-6fa6dec778da.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```python
sp=0
cp=0
pp=0
si=0
ci=0
pi=0
li=-1
ls=-1
n=-1
num=-1

while(li<0):
    li = int(input("Limite inferior: "))
    
    if(li<0):
        print("Tiene que ser mayor a 0")
        
while(ls<li):
    ls = int(input("Limite superior: "))
    
    if(ls<li):
        print("Tiene que ser mayor que el limite inferior")
        
while(n<0):
    n = int(input("¿Cuantos numeros? "))
    
    if(n<0):
        print("Tiene que ser mayor a 0")
    
for i in range(n): 
    while(num<=li or num>=ls):
        num = int(input("Dame un numero de LI y LS: "))
        
        if(num<=li or num>=ls):
            print("Tiene que estar dentro del LI al LS")

    if(num%2==0):
        sp=sp+num
        cp=cp+1
    else:
        si=si+num
        ci=ci+1
        
    num=-1       
         
if(sp==0 or cp==0):
    pp=0
else:
    pp=sp/cp
    
if(si==0 or ci==0):
    pi=0
else:
    pi=si/ci
    
if(pp>pi):
    print("El PP es mayor que el PI")
else:
    print("El PI es mayor que el PP")
```
**_Ciclo while:_**
```python
print("Dame Límite inferior: ")
Li = int(input())
while Li<0:
    print("El límite inferior debe ser mayor a 0")
    print("Dame Límite inferior: ")
    Li = int(input())

print("Dame límite superior: ")
Ls = int(input())
while Ls<=Li:
    print("El límite superior no puede ser menor o igual al limite inferior")
    print("Dame límite superior: ")
    Ls = int(input())

pares = 0
impares = 0

lista=[]
for x in range(10):
    valor=int(input("Ingrese un valor entero: "))
    lista.append(valor)
print(lista)

for a in lista:
    if a % 2 == 0:
        pares = pares + a
    else:
        impares = impares + a
print("La suma de los números pares es: ",pares)
print("La suma de los números impares es: ",impares)

prom_pares = pares / a
prom_impares = impares / a

print("El promedio de los números pares es: ",prom_pares)
print("El promedio de los números impares es: ",prom_impares)

if prom_pares > prom_impares:
    print("El promedio de los pares es mayor que el promedio de los impares.")
else:
    print("El promedio de los números impares es mayor que el promedio de los pares.")
```
**_Ciclo do-while:_**
```dart
void main() {
  double sumap = 0;
  double sumai = 0;
  var contp = 0;
  var conti = 0;
  double promp = 0;
  double promi = 0;
  print('Introduce el limite inferior, mayor a 0');
  var li = int.parse(stdin.readLineSync()!);
  if (li < 0) {
    print('tu limite inferior debe ser mayor a 0');
  }
  if (li > 0) {
    print('Ahora introduce un limite superior');
    var ls = int.parse(stdin.readLineSync()!);
    if (ls < li) {
      print('tu limite superior debe ser mayor a tu limite inferior');
    }
    var cont = li;
    do {
      if (cont <= ls) {
        sumai = sumai + cont;
        conti = conti + 1;
      }
      if (cont % 2 == 0) {
        sumap = sumap + cont;
        contp = contp + 1;
        sumai = sumai - cont;
        conti = conti - 1;
      }
      cont = cont + 1;
    } while (cont <= ls);

    promi = sumai / conti;
    print('los impares son $conti y su promedio es $promi');
    promp = sumap / contp;
    print('los pares son $contp y su promedio es $promp');
    if (promp < promi) {
      print('$promi es mayor');
    }
    if (promp > promi) {
      print('el promedio $promp es mayor');
    }
  }
}
```

#### 1.4 Entradas
Limite inferior y superior, números.
#### Salidas
Lista de números, promedios de los números pares e impares (por separado), y cuál promedio es mayor.



## **Ejercicio 9.**
#### Obtener la frecuencia de n calificaciones entre [1,10]. Indique la cantidad de aprobados, la cantidad de reprobados, el promedio de aprobados y promedio general.
#### 1.1 Análisis
Usar el símbolo de proceso para asignar un array para las calificaciones, pedir al usuario que ingrese las calificaciones, validar que estas esten entre 0 y 10, además de verificar en cada calificación ingressada si es mayor-igual a 6 para ingresar a las calificaciones aprobatorias, de lo contrario almacenar en las calificaciones reprobatorias, hacer las operacines correspondientes para obtener los promedios de las calificaciones aprobatorias y general , imprimir todo para finalizar.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E9_for](https://user-images.githubusercontent.com/113486125/198375938-41c64dba-5ff1-4520-b4cd-3fce7132bef3.png)

**_Ciclo while:_**

![E9_while](https://user-images.githubusercontent.com/113486125/198390942-490a416f-0774-4449-8c87-7ae43e8b6bdf.png)

**_Ciclo do-while:_**

![E9_dowhile](https://user-images.githubusercontent.com/113486125/198390978-e3a3240f-73c2-4960-9a1e-b3807d73b44b.png)

#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```python
Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0

for i in range(1,Calificaciones+1):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)

promedio=n/len(vec)

npromedio=0
for j in vec:
    if j>promedio:
        npromedio=npromedio+1

aprobado=0

#Primero inicializas el contador
promedioAprobados = 0
for h in vec:
    if h>5:
        aprobado=aprobado+1
        #Va sumando cada unas de las notas
        promedioAprobados = promedioAprobados + h

#Luego saca el promedio sumatoria / cantidad de aprobados 
promedioAprobados = promedioAprobados / aprobado

reprobado=0
for k in vec:
    if k<5:
        reprobado=reprobado+1

print("Max Calificacion", max(vec))
print("Min calificacion", min(vec))
print("Promedio:", promedio)
print("Superiores a promedio:", npromedio)
print("Cantidad de aprobados:", aprobado)
print("Promedio de aprobados:", promedioAprobados)
print("Desaprobados:", reprobado)
```
**_Ciclo while:_**
```python
Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0
cont = 0
while(cont < Calificaciones):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)
    cont += 1

promedio=n/len(vec)

npromedio=0
for j in vec:
    if j>promedio:
        npromedio=npromedio+1

aprobado=0

#Primero inicializas el contador
promedioAprobados = 0
for h in vec:
    if h>5:
        aprobado=aprobado+1
        #Va sumando cada unas de las notas
        promedioAprobados = promedioAprobados + h

#Luego saca el promedio sumatoria / cantidad de aprobados 
promedioAprobados = promedioAprobados / aprobado

reprobado=0
for k in vec:
    if k<5:
        reprobado=reprobado+1

print("Max Calificacion", max(vec))
print("Min calificacion", min(vec))
print("Promedio:", promedio)
print("Superiores a promedio:", npromedio)
print("Cantidad de aprobados:", aprobado)
print("Promedio de aprobados:", promedioAprobados)
print("Desaprobados:", reprobado)
```
**_Ciclo do-while:_**
```python
Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0

cont = 0
while(True):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)
    cont += 1
    if(cont>=Calificaciones):
        break;
        
aprobado=0

promedioAprobados = 0
for h in vec:
    if h>=5:
        aprobado=aprobado+1
        promedioAprobados = promedioAprobados + h

promedioAprobados = promedioAprobados / aprobado

reprobado=0
for k in vec:
    if k<=5:
        reprobado=reprobado+1

print("Cantidad de aprobados:", aprobado)
print("Cantidad de reprobados:", reprobado)
print("Promedio de aprobados:", promedioAprobados)
```

#### 1.4 Entradas
Calificaciones.
#### Salidas
cantidad de reprobados, cantidad de aprobados, promedio general y de aprobados.


#**_Ejercicios de repaso._**
##**Ejercicio 10.**
#### Ingresar dos números y di cuál es mayor.
#### Diagrama:

![E10](https://user-images.githubusercontent.com/113486125/198499421-95fc11ba-971d-4db2-84ea-7238c49c4684.png)

##**Ejercicio 11.**
#### Capture 10 números enteros positivos.
#### Diagrama:

![E11](https://user-images.githubusercontent.com/113486125/198499569-904e0331-79d6-4c7d-b9ba-81a98c071cae.png)

##**Ejercicio 12.**
#### Capture 10 números enteros positivos, diga cual es mayor y cual es menor.
#### Diagrama:

![E12](https://user-images.githubusercontent.com/113486125/198499603-e93f42f3-2b82-4057-9e6f-63c14683ba6b.png)

##**Ejercicio 13.**
#### Calcular la ditancia mayor de dos números consecutivos en una lista de 10 números.
#### Diagrama:

![E13](https://user-images.githubusercontent.com/113486125/198499644-9c62d0e8-6f8b-4c47-a8de-b3bac1819e9b.png)

##**Ejercicio 14.**
#### Escribe un dfd que escriba la siguiente forma:

#### Diagrama:

![E14](https://user-images.githubusercontent.com/113486125/198499683-ee945bf3-512d-456f-a42c-eaadd2d8035b.png)

