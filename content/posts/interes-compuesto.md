---
title: "Interés compuesto"
description: "Introducción a la siguiente entrada"
draft: false
date: 2023-01-21
---

## Interés compuesto

Una definición bastante precisa de lo que es interés compuesto lo da Llambías cuando dice:

> 695. ANATOCISMO: NOCIÓN.- ES la capitalización de los intereses, o interés compuesto, de modo que agregándose tales intereses al capital originario pasan a redituar nuevos intereses.

Esto es notable desde la misma notación de la fórmula. La del interés simple es:

$$
I = C \times \Delta t \times ratio
$$

Casi intuitivamente que esos valores constantes ---salvo el tiempo que pasa--- van a dibujar una recta en las coordenadas cartesianas, merced justamente a que el tiempo sucede instante tras instante:

Así si partimos desde un $C$ equivalente a 100 y un $ratio$ de 33% anuales:

![IntSimple](/posts/img/iss.png)

Una ecuación de primera grado siempre genera rectas.

La del interés compuesto es:

$$
V_f  = V_n (1 + i/f)^{(f n)}
$$

|      Simb. |  Obs.  |
| ------ | ------ |
| $$V_f$$ |	es el valor final.|
| $$V_n$$	| es el valor de un periodo determinado |
| $$i$$	| es la ratio del interés |
| $$n$$	| son los periodos |
| $$f$$	| es la frecuencia de actualización |

Ello asumiendo que la frecuencia es un número finito.

No hace falta estimar valor alguno para darse cuenta de que esa ecuación es una cuadrática. En el plano no nos dibujerá una recta: Veamos.

$$
V_f  = V_n (1 + i/f)^{(f n)}
$$

$$
V_f = 100 \cdot \left(1 + \dfrac{0.36}{{1}}\right)^{6 \times 1}
$$

$$
V_f = 100 \times 1.36 ^ {6 \times 1}
$$

$$
V_f = 100 \times 6.32 = 632
$$

![Interes](/posts/img/compuesto.png)

¿Es legal esto? Sí, claro. Siempre y cuando la llamada *tasa efectiva* no supere los límites usurarios. En el caso, lo hace. Así que para el mismo, no.
