# FLOPS y TFLOPS

En primer lugar indicar que lo correcto es hablar de **FLOPS** ya que **TFLOPS** es el mismo concepto medido en Teras; *1 TFLOPS = 1 FLOPS x 10<sup>12</sup>*



**FLOPS o Floating  Point Operations per Second**, son como bien indica su nombre,  las operaciones de coma flotante por segundo que puede realizar un equipo.

Hay diversas formas de medir los FLOPS de los componentes, en **tiempo real** y **sostenidos**, pero normalmente los fabricantes no especifican en cual se están basando. Normalmente se refieren al *tiempo real* ya que esto suele coincidir con el  **peak** máximo del componente, pero aun así es una información un tanto sesgada.

### ¿Por qué no se deben comparar componentes según sus TFLOPS?

La respuesta es porque básicamente esta medida no tiene en cuenta la **arquitectura** de cada componente, sino solo las unidades de cómputo y su frecuencia. Por lo que ignora parámetros importantes como el rendimiento de **entradas y salidas**, disposición de **cachés**, sus **latencias**, **ALUs**, **buses de datos**, etc.

Un ejemplo claro de la incertidumbre de esta medida es comprar la *RX 5700 XT* con la *RTX 2070*:

Para calcular sus TFLOPS usamos la siguiente fórmula:

*TFLOPS* = **shaders x 2 x frecuencia boost**

*RTX 2070* = **2304 x 2 x 1620 MHz --> 7.464.960 FLOPS => 7.465 TFLOPS**

*RX 5700 XT* = **2560 x 2 x 1905 MHz --> 9.753.600 FLOPS => 9.753 TFLOPS**

Como se puede observar hay una diferencia del **30,66%** de la *RX 5700 XT* respecto a la *RTX 2070*, pero en la práctica ambas gráficas rinden prácticamente idénticas.

Esta medida se aplica en muchos campos de la informática, así como **CPU, GPU, consolas, SoCs** (donde se suele sumar los  FLOPS de CPU y GPU), complicando aún más la forma de medir su rendimiento.