---
layout: post
title:  "Evaluación de Proyectos: Periodo de recuperación."
date:   2024-04-22 23:15:00 -0400
categories: Evaluación-de-Proyectos 
permalink: /:categories/:year/:month/:day/:title/
---

### Definición.
Es el período que se requiere para que una inversión genere _**flujos de efectivo**_ suficientes para recuperar su costo inicial. (Período que se requiere para recuperar la inversión inicial).

### Criterio de decisión.
Una inversión es aceptable si el período calculado es inferior al número de años previamente especificado.

### Periodo de recuperación descontado.
Es la cantidad de tiempo que debe transcurrir para que la suma de los _**flujos de efectivo descontados**_ sea igual a la inversión inicial.

El periodo de recuperación descontado considera el valor del dinero a través del tiempo.

### Ejemplo.
Se requiere de un rendimiento de 11.5% sobre las nuevas inversiones y se tiene una inversión de 400 dólares con un flujo de efectivo de 120 dólares por año, durante 5 años.

**Solucion.**\
La siguiente tabla nos permitirá ver el momento en que recuperamos la inversión.

| Año | FE   | FE desc. | FE ac. | FE desc. ac. |
|-----|------|----------|--------|--------------|
| 1   | $120 | $108     | $120   | $108         |
| 2   | $120 | $97      | $240   | $205         |
| 3   | $120 | $87      | $360   | $292         |
| 4   | $120 | $78      | $480   | $370         |
| 5   | $120 | $70      | $600   | $440         |

Donde:\
**FE**: Flujo de Efectivo.\
**FE desc.**: Flujo de Efectivo descontado.\
**FE ac.**: Flujo de Efectivo acumulado.\
**FE desc. ac.**: Flujo de Efectivo descontado acumulado.

Para el cálculo de **FE desc.** utilizamos la formula:

$$ FE_{desc} = \frac{FE}{(1 + i)^n} $$

Si el periodo límite para recuperar la inversión es 5 años observamos que se cumple con el criterio para el **flujo de efectivo** puesto que la inversión se recupera al cuarto año (columna **FE ac.**).

Si consideramos el requisito de rendimiento (11.5%) la inversión no cumple el criterio ya que se recupera al quinto año (columna **FE desc. ac.**).  
