---
layout: post
title:  "Evaluación de Proyectos: Valor actual neto."
date:   2024-05-02 13:10:00 -0400
categories: Evaluación-de-Proyectos 
permalink: /:categories/:year/:month/:day/:title/
---

### Definición.
Acrónimo **VAN**. Es el valor presente de los flujos netos de efectivos (ingresos – egresos) originados por una inversión.

<!--$$ VAN=\sum_{t=1}^{n}\frac{FE_{t}}{(1+i)^{t}}-I_{0} $$-->
![van](/assets/images/van.jpg)

Donde:\
FE_{t} : Flujo neto de efectivo en el periodo.\
i : Costo de oportunidad.\
n : Vida esperada del proyecto.\
I_{0} : Costo inicial del proyecto.

### Criterio de decisión.
Si el valor presente neto es positivo, el proyecto debe ser aceptado; si es negativo, debe ser rechazado.

Si dos proyectos son mutuamente excluyentes, el que tenga el valor presente neto más alto deber ser el elegido.

### Ejemplo.
Obtenga el VAN de cada uno de los proyectos de la tabla siguiente, considerando un costo de oportunidad de capital aplicable del 10%.

| Año | A       | B       | C       | D       |
|-----|---------|---------|---------|---------|
| 0   | -$1.500 | -$1.500 | -$1.500 | -$1.500 |
| 1   | $150    | $0      | $150    | $300    |
| 2   | $1.350  | $0      | $300    | $450    |
| 3   | $150    | $450    | $450    | $750    |
| 4   | -$150   | $1.050  | $600    | $750    |
| 5   | -$600   | $1.950  | $1.875  | $900    |

**Solución.**\
Utilizando una hoja de calculo calculamos el VAN para cada proyecto:

|     | A     | B    | C    | D    |
|-----|-------|------|------|------|
| VAN | -$610 | $766 | $796 | $779 |

El criterio de decisión nos señala que debemos excluir aquellos proyectos con VAN negativo y elegir el que presente mayor valor. Por tanto, **El proyecto C** será el seleccionado. 