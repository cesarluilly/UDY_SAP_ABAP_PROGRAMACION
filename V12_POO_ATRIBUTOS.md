##### Atributos

```abap
*&---------------------------------------------------------------------*
*& Report YLU_ATRIBUTOS_POO
*&---------------------------------------------------------------------*
*&
*&---------------------------------------------------------------------*
REPORT ylu_atributos_poo.

CLASS cls_factura DEFINITION.

  PUBLIC SECTION.
    DATA proveedor TYPE string.

*   Static Variable o Dato de Clase.
    CLASS-DATA static_fecha_pago TYPE d.

ENDCLASS.

START-OF-SELECTION.

  DATA: go_factura_1 TYPE REF TO cls_factura,
        go_factura_2 TYPE REF TO cls_factura.

  CREATE OBJECT: go_factura_1,
                 go_factura_2.

  go_factura_1->proveedor = 'DELL'.
  go_factura_2->proveedor = 'HP'.

  WRITE : / go_factura_1->proveedor.
  SKIP 2.
  WRITE : / go_factura_2->proveedor.
  skip 2.

* Para asignar/obtene valor a propiedad estatica se hace con signo '='
  cls_factura=>static_fecha_pago = '20250601'.
  WRITE : / go_factura_2->static_fecha_pago.
  WRITE : / cls_factura=>static_fecha_pago.
```
