
```abap
*&---------------------------------------------------------------------*
*& Report YLU_VARIABLES_INCOMPLETO
*&---------------------------------------------------------------------*
*&
*&---------------------------------------------------------------------*
REPORT ylu_variables_incompleto.

DATA cadena TYPE c LENGTH 4.

cadena = 'Hola'.

WRITE cadena.

DATA numero TYPE p LENGTH 10 DECIMALS 2.

numero = '45.20'.

* Con Diagonal imprimimos en una linea nueva.
WRITE / numero.

* Con dos puntos y comas podemos imprimir varias variables en un write
WRITE: cadena, 'Alumno ABAP'.
```
