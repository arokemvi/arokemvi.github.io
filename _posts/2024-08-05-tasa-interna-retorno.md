---
layout: post
title:  "Evaluación de Proyectos: Tasa interna de retorno"
date:   2024-08-05 15:44:00 -0400
categories: Evaluación-de-Proyectos 
permalink: /:categories/:year/:month/:day/:title/
---

### Definición.
La TIR se define como la tasa de interés que iguala el valor presente de los flujos de efectivo esperados a futuro, o de los ingresos, con el desembolso inicial de efectivo.

<!--$$ \sum_{t=1}^{n}\frac{FE_{t}}{(1+TIR)^{t}}-I_{0}=0 $$-->
![tir](/assets/images/tir.jpg)

Donde:\
FE_{t} : Flujo neto de efectivo en el periodo.\
n : Vida esperada del proyecto.\
I_{0} : Costo inicial del proyecto.

### Criterio de decisión.
Una inversión es aceptable si la TIR es superior al rendimiento requerido. De lo contrario, debería ser rechazada.

### Ejemplo.
Dado los siguientes flujos de efectivos y un rendimiento requerido del 10%, evaluar mediante la TIR si el proyecto es aceptable.

| Año | FE   |
|-----|------|
| 0   | -100 |
| 1   | 60   |
| 2   | 60   |

**Solución.**\
Utilizando una hoja de calculo podemos emplear el método gráfico para estimar el valor de la TIR.

La siguiente gráfica muestra el valor del VAN para tasas de rendimiento entre 0% y 20%. 

![TIR](/assets/images/TIR.png)

Para estimar La TIR buscamos el valor del eje x donde el VAN es cero, es decir:\
**TIR≈13%**

Como el rendimiento requerido para el proyecto es 10%, este es menor que la TIR por tanto según el criterio de decisión el proyecto **es aceptable**.
