```
*&---------------------------------------------------------------------*
*& Report YLU_EXPRESIONES
*&---------------------------------------------------------------------*
*&
*&---------------------------------------------------------------------*
REPORT ylu_expresiones.

DATA: numero_a TYPE i,
      numero_b TYPE i,
      numero_c TYPE i.

numero_b = 4.
numero_c = 6.

* BREAK cgarcia.

* Suma
WRITE: / 'A Original= ', numero_a.
ADD 2 TO numero_a.
WRITE: / 'A Add 2= ', numero_a.

CLEAR: numero_A,
      numero_b,
      numero_c.
WRITE: / 'A Clear = ', numero_a.

numero_b = 10.
numero_c = 7.

* Resta
numero_a = numero_b - numero_c.
WRITE: / 'A = ', numero_a.

SUBTRACT 1 FROM numero_a.
WRITE: / 'A = ', numero_a.

* Multiplicacion
numero_a = numero_b * numero_c.
WRITE: / 'A = ', numero_a.

MULTIPLY numero_a by 2.
WRITE: / 'A = ', numero_a.

numero_b = 8.
numero_c = 2.

* Division.
numero_a = numero_b / numero_c.
WRITE: / 'A = ', numero_a.

* Orden de operaciones matematicas.
numero_a = 2 * ( numero_b + numero_c ).
```
