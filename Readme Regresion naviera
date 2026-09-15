# Regresión Lineal para la Valoración de Activos en la Industria Naviera

Análisis estadístico aplicado a la toma de decisiones de compra en el sector de transporte marítimo de carga, usando regresión lineal múltiple sobre datos reales de transacciones de buques (2007–2008).

*Trabajo académico — Universidad EAFIT, 2022. Coautoría: Laura Valencia Giraldo y Simón Higuita Cortés.*

## Contexto del negocio

La industria naviera presenta alta volatilidad en el precio de sus activos. Un ejemplo real que motivó este análisis: en 2007 un comprador adquirió el buque *Cape Kassos* por USD 100 millones, y 13 meses después lo revendió (renombrado *Nightfight*) por USD 158 millones.

Sin un modelo objetivo de valoración, decisiones de esta magnitud dependen de la inspección física y el criterio subjetivo del comprador. Este proyecto plantea un modelo cuantitativo para estimar el precio justo de un buque a partir de sus características.

## Metodología

Se aplicó **regresión lineal múltiple** sobre una base de datos de transacciones históricas (enero 2007 – mayo 2008), usando como variables:

- **Y** — Precio de venta (USD millones)
- **X1** — Antigüedad del buque (años)
- **X2** — Capacidad de carga / peso muerto (toneladas)
- **X3** — Índice Baltic Dry (Capesize) del mes de la transacción

**Modelo resultante:**

```
Y = 44.22 − 2.45·X1 + 0.24·X2 + 0.007·X3
```

## Validación del modelo

Se probó el modelo contra transacciones reales fuera de la muestra de entrenamiento:

| Buque | Precio real | Precio estimado | Error |
|---|---|---|---|
| Buque 1 | — | USD 82.58 M | 13.12% |
| Buque 2 | — | USD 41.38 M | 8.03% |

El modelo también se usó para simular escenarios: dos buques con la misma antigüedad y año de construcción, pero distinta capacidad de carga (130 vs. 195 toneladas), arrojaron precios estimados de USD 111.11 M y USD 126.85 M respectivamente — confirmando la relación lógica entre capacidad y valor del activo.

## Hallazgos clave

- La capacidad de carga (X2) es la variable con mayor peso económico en el valor del buque.
- El modelo captura razonablemente bien la relación precio-características, con errores de estimación entre 8% y 13% frente a transacciones reales — un margen aceptable dado el nivel de fluctuación propio del mercado naviero.
- Un modelo de regresión no reemplaza el criterio experto, pero reduce significativamente el riesgo de sobre/subvalorar un activo frente a decisiones basadas solo en inspección física.

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `data/base_datos_transacciones.xlsx` | Dataset histórico de transacciones de buques (2007–2008) |
| `analysis/calculo_regresion.xlsx` | Cálculo del modelo de regresión lineal múltiple |
| `docs/caso_compass_maritime.pdf` | Descripción del caso de negocio (Compass Maritime Services LLC) |

## Herramientas utilizadas

Excel (Análisis de Datos / Regresión) · Estadística descriptiva e inferencial · Modelos de regresión lineal múltiple

## Habilidades aplicadas

Análisis de datos · Modelado estadístico · Interpretación de resultados para toma de decisiones de negocio · Validación de modelos

