
```abap
*&---------------------------------------------------------------------*
*& Report YLU_CONSTANTES
*&---------------------------------------------------------------------*
*&
*&---------------------------------------------------------------------*
REPORT ylu_constantes.

DATA numero TYPE i.

numero = 4.

WRITE: 'El valor de la variables es = ', numero.

numero = 3.

WRITE: / 'El valor de la variables es = ', numero.

* 2 digitos para Hora, minutos, segundos
CONSTANTS: hora type t VALUE '143050',
          nombre type string value 'Cesar'.

write: / hora ENVIRONMENT TIME FORMAT,
       / nombre.
```
