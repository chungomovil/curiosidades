# T-Case

Siempre hablamos de parámetros conocidos por todos como la temperatura, el rendimiento o el consumo cuando nos referimos a un procesador. Pero hay otros parámetros menos conocidos que son muy útiles a la hora de relacionar cualquiera de estos términos y que nos ayudan a comprender otros conceptos de una CPU. 

Uno de ellos es el llamado **TCase**, algo que solo incluyen las CPU Intel y que es muy útil en según qué situaciones.

Como bien sabemos, tanto Intel como AMD se esfuerzan en ser precisos a la hora de reflejar conceptos como la temperatura o el consumo, todo mediante sensores que pueden estar situados en el propio procesador o en la placa base.

## TCase, cuando la temperatura tiene límite en un componente concreto

<img src="https://hardzone.es/app/uploads-hardzone.es/2020/05/Tcase-Intel.jpg" alt="Tcase-Intel" style="zoom: 80%;" />

**TCase** es, como su propio nombre indica, la **temperatura de la carcasa**, entendiendo por ello la temperatura que máxima permitida en el **difusor de calor integrado** de la CPU, también conocido como **IHS**. Es decir, es la temperatura máxima que el IHS puede soportar.

Sirve como medida para los fabricantes de disipadores o bloques de CPU/AIO.  De esta manera, se puede determinar la temperatura máxima que puede soportar el IHS sin que el die sufra riesgos de rotura, Throttling o pérdidas de rendimiento y se asegura que en todos los puntos del IHS nunca se deba llegar a dicho valor.

## Un valor que es mas bajo que Tjmax e igual de importante

<img src="https://hardzone.es/app/uploads-hardzone.es/2020/05/Intel-TCase.jpg" alt="tjcase-tjunction" style="zoom: 50%;" />

Normalmente, **TCase** tiene de media un valor bastante inferior al que reporta **Tjmax** o los propios núcleos, sin embargo, *algunos software unifican ambas temperaturas o hacen una media de las dos*.

**El problema es que TCase por su naturaleza es bastante más fresco que Tjmax**, normalmente y dependiendo de la arquitectura e IHS, sobre 10 a 20 grados más frío. Por ello, esta **TCase** solo es usada por fabricantes, ya que pretenden comprobar si sus soluciones de enfriamiento son capaces de solventar y enfriar por debajo de su valor máximo.

Esto es algo muy común en equipos OEM, los cuales van buscando la rentabilidad en cada componente para ofrecer precios bajos y como tal, pretenden ir al límite de este tipo de valores.

![ihs-intel](https://hardzone.es/app/uploads-hardzone.es/2020/05/Intel_Pentium_4_2.80A-4014.jpg)

Intel hasta hace no demasiado tiempo tenía una forma muy curiosa de medir este **TCase** y no era más que hacer un pequeño agujero en el IHS sin que llegase a traspasarlo, donde en sus instalaciones entraba una sonda de forma perfecta y podían medir si cada CPU ofrecía valores correctos, lo que evidenciaba que la soldadura o TIM estaba haciendo un contacto correcto.



Esto se ha suprimido en los procesadores actuales, hasta el punto de que el gigante azul ya no especifica **TCase** entre los valores de sus CPU, **por lo que todo se reduce a Tjunction o Tjmax**.