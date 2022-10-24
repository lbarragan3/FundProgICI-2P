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
```
void main(List<String> args) {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s");
}
```
**_Ciclo while:_**
```
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
```
**_Ciclo do-while:_**
```
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
