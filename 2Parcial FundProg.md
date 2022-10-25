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

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("la suma de numeros pares es:$s");
}
```
**_Ciclo do-while:_**
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
```

```
**_Ciclo while:_**
```

```
**_Ciclo do-while:_**
```

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
```
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}
```
**_Ciclo while:_**
```
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
```
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
```
listanumeros = []
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)

print(f"los numeros son {listanumeros}")

def pares(listanumeros):
    listanumeros = []


for n in listanumeros:
    if n % 2 == 0:
        print("Estos numeros son pares"+ "  " + str(n))
```
**_Ciclo while:_**
```
listanumeros = []
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
decision = input("¿desea añadadir mas numeros?: ")

while decision == "s" or decision == "s":
    numerousuario = int(input("introdusca otro numero: "))
    listanumeros.append(numerousuario)
    decision = input("¿desea añadir otro numero?: ")


print(f"los numeros son {listanumeros}")
for n in listanumeros:
    if n % 2 == 0:
        print("Este numero de la lista es par" + str(n))
        


input("por favor, precione una tecla para salir.")
```
**_Ciclo do-while:_**
```
print("PARES")
numero_1 = int(input("Escriba un número entero: "))
numero_2 = int(input(f"Escriba un número entero mayor o igual que {numero_1}: "))

if numero_2 < numero_1:
        print(f"¡Le he pedido un número entero mayor o igual que {numero_1}!")
else:
        for i in range(numero_1, numero_2 + 1):
            if i % 2 == 0:
                print(f"El número {i} es par.")
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
```

```
**_Ciclo while:_**
```

```
**_Ciclo do-while:_**
```

```

#### 1.4 Entradas
Calificacines
#### Salidas
Calificaciones, promedio de las calificaciones aprobatorias y cantidad de alumnos reprobados.


## **Ejercicio 8.**
#### Capture n números en el rango [Li,Ls] donde: -Li = Limite inferior -Ls limite superior para li<ls y l0, obtenga: Cantidad de números pares y su promedio, Cantidad de números impares y su promedio y ¿Qué promedio es mayor?
#### 1.1 Análisis
[Texto]
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**


**_Ciclo while:_**


**_Ciclo do-while:_**


#### 1.3 Códigos (python, dart o C):
**_Ciclo for:_**
```

```
**_Ciclo while:_**
```

```
**_Ciclo do-while:_**
```

```

#### 1.4 Entradas
Ninguna
#### Salidas
30
