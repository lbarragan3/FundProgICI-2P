# **Ejercicios de Clase**
### **Resolución de problemas de clase con Diagramas de Flujo de Datos**
## **Ejercicio 1.**
#### Contar del 1 al 10 y sumar los valores.
#### 1.1 Análisis
Usar el símbolo de proceso para dar valor a la variable suma, además de realizar un contador donde los números deberan de cumplir con la condición, si estos ecceden las condiciones establecidas imprimir el contador para finalizar.
#### Diagrama ciclo for:
#### 1.2 Diagrama de Flujo de Datos:
**_Ciclo for:_**

![E1_for](https://user-images.githubusercontent.com/113486125/197437734-43b0661a-f79c-4ce4-9ffb-a7bc608efe89.png)

**_Ciclo while:_**

![E1_while](https://user-images.githubusercontent.com/113486125/197439568-511655c5-ef95-475a-8167-ed751d521d96.png)

**_Ciclo do-while:_**

![E1_dowhile](https://user-images.githubusercontent.com/113486125/197439608-90fe5d1c-41bd-4fc8-983f-25db88d3300a.png)

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

![2DO PROBLEMA FOR](https://user-images.githubusercontent.com/113486125/197451333-9b4e4126-0c5f-433c-967c-cde69c6db35b.jpg)

**_Ciclo while:_**

![2DO PROBLEMA WHILE](https://user-images.githubusercontent.com/113486125/197451367-7bba1cd2-3565-49bd-ab36-4fcad36870ef.jpg)

**_Ciclo do-while:_**

![2DO PROBLEMA DO WHILE](https://user-images.githubusercontent.com/113486125/197451381-f91f122d-581a-442e-9cc5-0da10acbf66d.jpg)

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

![3ER PROBLEMA FOR](https://user-images.githubusercontent.com/113486125/197452501-9861d725-8a7c-4a46-a8ea-15ad1d2ba494.jpg)

**_Ciclo while:_**

![3ER PROBLEMA WHILE](https://user-images.githubusercontent.com/113486125/197452519-413072b8-f05c-41b5-88e3-d9de49a3be75.jpg)

**_Ciclo do-while:_**

![3ER PROBLEMA DOWHILE](https://user-images.githubusercontent.com/113486125/197452547-2a93f599-c78f-4ecc-8427-dca7e533c71f.jpg)

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
