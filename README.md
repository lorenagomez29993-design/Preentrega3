# Checkpoint 2 - Power BI

## Medidas creadas

### 1. Total Ventas
Calcula el importe total de las ventas realizadas.

### 2. Total Costos
Calcula el costo total asociado a las ventas.

### 3. Total Transacciones
Cuenta la cantidad de registros de la tabla de hechos.

### 4. Clientes Únicos
Cuenta la cantidad de clientes distintos registrados en las ventas.

### 5. Utilidad Bruta
Calcula la diferencia entre el Total de Ventas y el Total de Costos.

### 6. Margen Bruto %
Calcula el porcentaje de utilidad sobre el total de ventas utilizando la función DIVIDE.

### 7. % Ventas sobre Total
Calcula qué porcentaje representa cada producto respecto del total de ventas, ignorando el filtro de producto mediante la función ALL.

### 8. Ventas Año Anterior
Calcula el total de ventas del mismo período del año anterior utilizando la función SAMEPERIODLASTYEAR.

### 9. Crecimiento Ventas %
Calcula el porcentaje de crecimiento de las ventas respecto del año anterior.

---

## Diferencias entre el diagrama del Checkpoint 1 y el modelo real

No se encontraron diferencias significativas entre el diagrama y el modelo implementado. Se mantuvo un esquema en estrella compuesto por una tabla de hechos (Hechos_Ventas) y la tabla de fechas (Fechas), con una relación de uno a muchos. Además, se organizó la totalidad de las medidas DAX en la tabla _Medidas para facilitar el mantenimiento del modelo.

---

## Prueba de Contexto

Se creó una página denominada **Prueba de Contexto** que contiene:

- Una tarjeta con la medida **Total Ventas**.
- Una tabla con **Producto**, **Total Ventas**, **Margen Bruto %** y **% Ventas sobre Total**.
- Un segmentador por **Año** conectado a la tabla **Fechas**.

Decisiones de diseño
Se utilizaron tarjetas para destacar los KPIs principales y facilitar una lectura rápida.
Se eligió un gráfico de líneas para mostrar la evolución temporal de las ventas.
Se utilizaron barras horizontales para comparar el Margen Bruto entre productos.
Rol RLS

Se creó el rol Vista_Restringida, que limita la visualización únicamente al producto "Monitor".

Actualización programada

No aplica, ya que el dataset utiliza datos locales y no posee una fuente externa conectada.
