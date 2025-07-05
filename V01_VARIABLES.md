# Variables

```abap
*&---------------------------------------------------------------------*
*& Report YLU_VARIABLES_L100000
*&---------------------------------------------------------------------*
*&
*&---------------------------------------------------------------------*
REPORT YLU_VARIABLES_L100000.

* Declaracion de variables tipo fecha
DATA fecha type d.
DATA IVA type i.
DATA enterprise type string.

fecha = '20201127'.
iva = 18.
enterprise = 'Logali'.

write fecha.
write fecha DD/MM/YYYY.
write iva.
write enterprise.
```
