---
title: "¿Que debe saber un juez?"
description: "O, dicho de otro modo: ¿Qué se supone que sabe?."
draft: true
date: 2023-01-21
---

## Saber común.

Usualmente ello está contenido dentro de lo que el Código llama los hechos notoriamente conocidos.

¿Por ejemplo? ¿Literatura? Tal vez no. Tal vez no sepan ubicar la cita:

> <<A tí también, en lejanas playas de oro,
>
> Te aguarda incorruptible tu tesoro,
>
> La vasta vaga populosa muerte.>>

Pero deberían saber que es un terceto porque... ¿no pasaron por la secundaria?

Y tal vez no sea necesario que sepan demostrar que $$\sqrt{2}$$ es, en efecto un número irracional. Pero deberían saber lo que es uno si no falsificaron su diploma de bachiller.

Y es ahí donde quiero llegar. ¿Deberían conocer la fórmula del interés compuesto? ¿Deberían saber que es una simplificación de la _real_ fórmula?

El BCP tiene una calculadora en su página del método francés. Pero el BCP no tiene porque saber los hechos notorios. Pero el Juez sí.

La forma de distribuir los pagos de capital e intereses es la siguiente:

$$
a = \frac{C}{a_{|\overline{{n}}i}}
$$

Donde:

| --- | --- | --- |
| $$a$$ | , |es el término amortizativo del préstamo, en este caso, meses.   | 
| $$C$$ | , |es el capital prestado.    |
| $$i$$ | , |es el tipo de interés del préstamo.|
| $$n$$ | , |es el número de meses que dura el préstamo.|

$$
a_{|\overline{{n}}i} = \frac{(1+i)^n - 1}{i \times (1+i)^n}
$$

Luego:

\begin{equation}

a = \dfrac{C}{\dfrac{(1+i)^n - 1}{i \times (1+i)^n}} \rightarrow a = C \times 

\dfrac{i \times (1+i)^n}{(1+i)^n - 1}
    \end{equation}

    y, si sustituimos por los valores tenemos el monto de las cuotas:

    \begin{equation}
        a = \text{G.} 209.939.912 \times \dfrac{0,0175 (1+0,0175)^{72}}{(1+0,0175)^{72} - 1} = \text{G.} 5.151.085
    \end{equation}

    Como se observa, el interés va incluido en las cuotas desde el inicio de manera que el capital vaya amortizándose en razón de $(i+1)$. Y el resto se inpute a intereses\footnotemark. El sistema, como se ve, no es incompatible con la forma de inputar intereses del \CC{}.

    \footnotetext{No expreso la razón de los decrecientes pagos de intereses para no usar matemáticas que no sean las propias del Segundo Curso de la Educación Media: cálculo se empieza a dar en el Tercero. Además, como se verá enseguida, podemos suputarlo por un medio sencillo que solamente calcule las sumas de la progresión geométrica de las imputaciones al capital, calculando luego los pagos en concepto de interés por la diferencia.}

    Conocer qué parte de la primera cuota es pago de intereses es relativamente simple. Sólo tendríamos que calcular el interés mensual sobre el capital ya que en ese momento no hay aun ningún pago del mismo. Así que:

    \[ m = 5.151.085 \times \frac{21\%}{12}  = 1477136
    \]

    Con este dato, el primer término de nuestra serie, podemos conocer la cantidad de capital amortizado por las cuotas pagadas, que en el caso son 10. La suma de estos términos está dada por la siguiente fórmula:

    \setcounter{equation}{0}

    \begin{equation}
        S_{n} = a_{1} \cdot \frac {r^{n+1} -1 }{r-1}
    \end{equation}

    \begin{equation}
        S_{n} = 1477136 \cdot \frac { (0.0175+1)^{11} - 1 } {(0.0175+1)-1} = 17747600
    \end{equation}

    El Banco Central del Paraguay tiene una calculadora del método en \url{https://www.bcp.gov.py/calculadora}. Si se consulta, se notará que arroja una diferencia de 35 G. Se debe a los sucesivos redondeos que no se pueden evitar al hacer una tabla.

    Con ese dato, y sabiendo que 10 cuotas equivalen a $ 10 \times 5151085 = 51510850$, sabemos que se ha pagado $ 51510850 - 17747600 = $ de intereses y que las restantes cuotas contienen el resto de ellos.

    Sin embargo el documento que se presenta como <<pagaré a la orden>> dice:

    \begin{quote}
        <<MORA: La falta de pago de una cualesquiera de las cuotas indicadas más abajo a su vencimiento, producirá la mora de pleno derecho de toda la obligación principal, sin necesidad de protesto ni de ningún requerimiento judicial o extrajudicial y además, surtirá los siguientes efectos: a) Desde la fecha de la mora hasta la del efectivo pago, la obligación devengara un interés moratorio \textbf{sobre el saldo de la deuda} a la misma tasa del interés compensatorio aplicable en ese momento, más un interés punitorio adicional equivalente al treinta por ciento (30\%). más IVA de la tasa a percibirse en concepto de interés moratorio.  >>

    \end{quote}

    Lo cual no tiene sentido porque no se pueden capitalizar intereses en una misma operación. Y eso les esta prohibido a las Cooperativas. Porque lo suelen hacer seguramente, basado en la detallada descripción que hace el INCOOP de la prohibición  ---he agregado negritas:

    \begin{quote}
        <<En caso de morosidad, el interés a percibir por parte de la cooperativa a partir de la
    mora, denominado interés moratorio, será la misma tasa compensatoria pactada    originalmente. En ningún caso podrán capitalizarse intereses. Las cooperativas
    podrán percibir igualmente un interés punitorio adicional, calculado sobre el saldo
    de la deuda vencida, cuya tasa no podrá exceder del treinta por ciento (30\%) de la
    tasa a percibirse en concepto de interés moratorio. Para este efecto, tanto los intereses
    moratorios y punitorios se calcularán \textit{sobre el capital incluido en la cuota vencida }y por los
    dias de mora.>>\footnotemark

    \end{quote}


