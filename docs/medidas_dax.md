# Medidas DAX Utilizadas

Este documento describe las principales medidas DAX empleadas en el dashboard de Online Retail 2011.

---

## Ventas Totales

Calcula el ingreso total generado por todas las ventas.

```DAX
Ventas Totales =
SUM(df[Income])
```

---

## Número de Clientes

Cuenta los clientes únicos.

```DAX
Clientes =
DISTINCTCOUNT(df[CustomerID])
```

---

## Número de Pedidos

Cuenta los pedidos únicos realizados.

```DAX
Número de Pedidos =
DISTINCTCOUNT(df[InvoiceNo])
```

---

## Ticket Promedio

Calcula el valor promedio por pedido.

```DAX
Ticket Promedio =
DIVIDE([Ventas], [Pedidos])
```