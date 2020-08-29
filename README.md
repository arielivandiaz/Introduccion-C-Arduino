# Introduccion-C-Arduino



## Sintaxis

### Comentario en una linea "//"
```c
  // Esto es un comentario de un reglón
```

### Comentario de varias lineas "/* */"
```c
/** Esto es un comentario
					de varias lineas **/

```
### Headers 
```c
// #define  	- Definición de una variable/rutina constante
#define pi 3.1415

// #include 	 - Inclución de librerias
#include<math.h>

```

###  Fin de la sentencia ";" 
```c
a=5;
b=5+a;
```

###   Limites de un bloque "{}"
```c
if(a>b){  // Bloque de más  de una linea necesito corchetes
			mayor=a;
			b=0;
		}

if(a>b) mayor=a; //Una sentencia unica  no necesita corchetes
```
## Variables 

### Números Enteros
```c
  int my_variable = 8; //Número entero entre -32768 y 32768 en procesadores de 16 bits y -2147483648 y 2147483647 en procesadores de 32 bits
  unsigned int my_variable = 8; //Número entero entre 0 y 65535 en procesadores de 16 bits y 0 y 4294967295 en procesadores de 32 bits
  short my_variable= 8; //Número entero entre -32768 y 32768
  long my_variable = 8; //Número entero entre -2147483648 y 2147483647
  unsigned long my_variable = 8; //Número entero entre 0 y 4294967295
  byte my_variable = 8; //Número entero entre 0 y 255
```

### Números Decimales
```c
  float my_variable = 3.1415926; //Números decimales entre -3.4028235E+38 y +3.4028235E+38 con 4 bytes de precisión
  double my_variable = 3.1415926; //Números decimales entre -3.4028235E+38 y +3.4028235E+38 con 8 bytes de precisión
```
### Caracteres
```c
  char my_variable = 'a'; //Caracter ASCII
  char my_variable[] = "Hello World';  // Arreglo de caracteres
  char my_variable[11] = { 'H','e','l','l','o',' ','W','o','r','l','d','\0'}; //Misca declaración que la anterior con declaración completa
```

El tamaño de las variables es importante porque en un microcontrolador la memoria es limitada. Dependiendo del procesador los distintos tipos de variables pueden ser comunmente de 16, 32 o 64 bits. Como regla general se aplica:

| Tipo  | Tamaño  |
|---|---|
| int | 16 bits   |
| unsigned int | 16 bits  |
| short | 16 bits  |
| long  |  32 bits  |
| byte |  8 bits  |
| float  | 32 bits  |
| double | 64 bits  |
| char  | 8 bits  |
|   |   |

## Operadores 
###  Operadores Aritméticos Básicos
```c
//  Asignación "="
				a = 5;
//  Adición "+"
			b =a + 5;
//  Substracción "-"
			b = a - 3;
//  Multiplicación "*"
			b = a * 2;
//  División "/"
			b = a / 2;
//  Modulo "%"
			b = a % 2;
```

###  Operadores Comparación
```c
//	Igual a... "== "
//	Distinto de... "!="
//	Menor que... "<"
//	Mayor que... ">"
//	Menor o igual que... "<="
//	Mayor o igual que... ">="
```


###  Operadores Booleanos
```c
 //	and "&&"
	if(temp>30 && temp<45) 
			Serial.println("Todo va bien");
 
 //	or "||"
	if(temp<30 || temp>45)  
		Serial.println("Hay problemas");


 //	not "!"
	encendido=0;  //Ventilador apagado
	if(!encendido && temp>45){
		encendido=1;
		Serial.println("Vent encendido"); 
	}
```
###  Operadores Compuestos
```c
//	Incremento "++"
			a++;
//	Decremento "--"
			b--;
//	Suma compuesta "+="
			a+=5;
//	Resta compuesta "-="
			b-=a;
//	Multiplicacion compuesta "*="
			a*=4;
//	Division compuesta "/="
			a/=(b+5);
```
###  
```c

```
###  
```c

```
###  
```c

```
