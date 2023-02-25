---
title: "Liquidaciones"
description: "Hay mucho por hacer"
draft: true
date: 2023-01-21
---

Nuestro  C.C. define las tasas de interes de manera muy deficiente.

Interrogue el Código de Vélez. Parace mas interesado en definir su concepcion del dinero, errada como todas, pero no tan errada como otras que 

Una definición bastante precisa de lo que es interés compuesto lo da Llambías cuando dice:

> 695. ANATOCISMO: NOCIÓN.- ES la capitalización de los intereses, o interés compuesto, de modo que agregándose tales intereses al capital originario pasan a redituar nuevos intereses.

Esto es notable desde la misma notación de la fórmula. La del interés simple es:

$$
I = C \times \Delta t \times ratio
$$

Casi intuitivamente que esos valores constantes ---salvo el tiempo que pasa--- van a dibujar una recta en las coordenadas cartesianas, merced justamente a que el tiempo sucede instante tras instante:

Así si partimos desde un 

$$
C = 100
$$

y

$$
ratio = 33%
$$

![IntSimple](/posts/img/iss.png)

Una ecuación de primera grado siempre genera rectas.

La del interés compuesto es:

$$
V_f  = V_n (1 + i/f)^{(f n)}
$$

Nótese que no se trata de hallar la ratio de interés ya que tal ratio cambia de momento a momento, sino de hallar el Valor Final del Valor Inicial.

|       |  |  |
| ------  | --- |------ |
| $$V_f$$ | ; |	es el valor final.|
| $$V_n$$	| ; | es el valor de un periodo determinado |
| $$i$$	  | ; | es la ratio del interés |
| $$n$$	  | ; | son los periodos |
| $$f$$	  | ; | es la frecuencia de actualización |

Ello asumiendo que la frecuencia es un número finito.

No hace falta estimar valor alguno para darse cuenta de que esa ecuación es una exponencial. En el plano no nos dibujará una recta: Veamos.

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

Y siempre y cuando la persona a cuyo favor se generan tales intereses no sea un banco o financiera.

La orgánica del BCP decía antes:

> El interés a partir de la mora, denominado interés moratorio, será la misma tasa pactada originalmente. No podrán capitalizarse intereses moratorios por períodos inferiores a 30 (treinta) días.

Pero una modificación posterior borra toda posibilidad de que se capitalicen intereses.

Continúa en [¿Qué debe saber un Juez?](https://villalba.is/posts/que-debe-saber-un-juez/)










---
