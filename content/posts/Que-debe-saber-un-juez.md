---
title: "¿Que debe saber un juez?"
description: "O, dicho de otro modo: ¿Qué se supone que sabe?."
tags: ["saber", "matemáticas", "interés"]
draft: false
date: 2023-01-25
---

*Antes de leer este post, es mejor leer el de interés compuesto.*

**Saber común.**


Usualmente ello está contenido dentro de lo que el Código llama los hechos notoriamente conocidos.

¿Por ejemplo? ¿Literatura? Tal vez no. Tal vez no sepan ubicar la cita:

```
<<A tí también, en lejanas playas de oro,
Te aguarda incorruptible tu tesoro,
La vasta vaga populosa muerte.>>
```

Pero deberían saber que es un terceto porque... ¿no pasaron por la secundaria?

Y tal vez no sea necesario que sepan demostrar que $$\sqrt{2}$$ es, en efecto un número irracional. Pero deberían saber lo que es uno si no falsificaron su diploma de bachiller.

Y es ahí donde quiero llegar. ¿Deberían conocer la fórmula del interés compuesto? ¿Deberían saber que es una simplificación de la _real_ fórmula? El Mec entiende que es cuestión del [Primer Año de la Media](https://www.mec.gov.py/cms_v2/adjuntos/13208)

El BCP tiene una calculadora en su página del método francés. En ella parece sugerir que lo usen los bancos y financieras. Pero el BCP no tiene porque conocer los hechos notorios. El Juez sí.

La forma de distribuir los pagos de capital e intereses es la siguiente:

$$
a = \frac{C}{a_{|\overline{{n}}i}}
$$

Donde:
| |  |  Obs. |
| --- | --- | --- |
| $$a$$ | , |es el término amortizativo del préstamo, en este caso, meses.   | 
| $$C$$ | , |es el capital prestado.    |
| $$i$$ | , |es el tipo de interés del préstamo.|
| $$n$$ | , |es el número de meses que dura el préstamo.|

$$
a_{|\overline{{n}}i} = \frac{(1+i)^n - 1}{i \times (1+i)^n}
$$

Luego:

$$
a = \dfrac{C}{\dfrac{(1+i)^n - 1}{i \times (1+i)^n}} \rightarrow a = C \times \dfrac{i \times (1+i)^n}{(1+i)^n - 1}
$$

Como se observa, el interés va incluido en las cuotas desde el inicio de manera que el capital vaya amortizándose en razón de

$$
(i+1)
$$

Y el resto se inpute a intereses. El sistema francés no es incompatible con la forma de inputar intereses del Código Civil.

Es incompatible solamente con la Ley del Banco Central.

   
