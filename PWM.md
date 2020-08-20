# Qué es el PWM de un ventilador o bomba y cómo funciona

Desde hace bastantes años, tanto los ventiladores de gama media y alta como también las placas bases, disponen de un **sistema de control y regulación de la velocidad de giro para ventiladores y bombas** llamado **PWM** *(pulse-width modulation o modulación por ancho de pulsos).*

### La evolución de los ventiladores y bombas ha sido muy bien recibida

![PWM](https://hardzone.es/app/uploads-hardzone.es/2019/10/PWM-5.jpg)



Hace dos décadas los ventiladores utilizaban para su conexión **los cables típicos de tierra y 12V**, marcados como un cable negro y otro rojo, y en donde **las placas no podían regular la entrega de voltios como tal, por ello siempre funcionaban al máximo.**

La regulación llegó más tarde, donde se ofrecían **5V, 7V y 12V**, tras lo cual se implementó un **tercer cable y nuevo conector** llamado comúnmente **"3 pines"**. Dicho cable y conector **permitían un control de las revoluciones del ventilador mediante su voltaje**, pudiendo saber hasta que punto pueden girar estos.

![PWM-3](https://hardzone.es/app/uploads-hardzone.es/2019/10/PWM-3.jpg)



Este conector se implementó en las primeras bombas de refrigeración líquida custom hace más de 10 años y significó el **primer sistema de monitorización del rendimiento de estas,** lo mismo ocurría con los ventiladores.

La revolución llegó con la implementación del **PWM**, tecnología que ha hecho más por el mundo de la refrigeración líquida en general (AIO incluida) que por el de los ventiladores.

<img src="https://hardzone.es/app/uploads-hardzone.es/2019/10/PWM-4.jpg" alt="PWM-4" style="zoom: 67%;" />

 

- **Cable negro**: Tierra.
- **Cable Rojo:** Voltaje.
- **Cable Amarillo**: Sensor (se emplea para saber a cuantas RPM está girando el ventilador)
- **Cable Azul**: PWM o control.

*No siempre se cumplen los mismos colores.*



**PWM** es el acrónimo de **Pulse Width Modulation** y es un término extendido en cualquier sector que tenga que ver con la electrónica.

La función de *PWM* dentro de un ventilador o bomba de agua es la de hacer como una especie de interruptor (**gate**), ya que lo que se consigue es una **conexión y desconexión de energía a cada pulso.**

Este sistema lo que permite es **una regulación de la cantidad de energía que le llega a cada ventilador o bomba**, la cual **va desde 0 voltios hasta los 12 voltios en un PC**. El motor es alimentado por lo tanto por pulsos de potencia, donde **a menor tiempo entre pulsos mayor energía llega al ventilador o bomba.**

<img src="https://hardzone.es/app/uploads-hardzone.es/2019/10/pwm-ciclotrabajo.jpg" alt="pwm-ciclotrabajo" style="zoom: 80%;" />

Lo que tenemos que tener en cuenta es que la regulación **PWM no implica regulación de voltaje en sí misma, ya que siempre se suministran 12V.**

Los pulsos son los que regulan la energía que llega, por ello a menor tiempo entre pulsos mayor energía llega e inversa. Por ello **solo se recomienda conectar como máximo dos ventiladores por puerto PWM con 4 pines**.

<img src="https://hardzone.es/app/uploads-hardzone.es/2019/10/PWM-7.jpg" alt="PWM-7" style="zoom: 67%;" />

Esto viene influenciado en los splitter típicos, donde al pasar de dos controladores (hasta 9 que es el máximo actual) **solo hay un conector PWM real, mientras que el resto son de 3 pines.** **El ventilador maestro** (conectado al puerto con 4 pines) **sincroniza su señal con los ventiladores esclavos** (conectados a los puertos de 3 pines).

### Curiosidades del PWM

*PWM* como tecnología tiene una serie de curiosidades que en muchas ocasiones van ligadas a las bombas de agua. Por ejemplo, las bombas actuales necesitan una serie de vatios que un cable de 4 pines no puede suministrar y por lo tanto **requieren un molex o SATA como alimentación adicional.**

<img src="https://hardzone.es/app/uploads-hardzone.es/2019/10/PWM-6.jpg" alt="PWM-6" style="zoom: 67%;" />

Esto implica que, que en estos dispositivos, **el cable de 4 pines solo tendrá dos**, dejando la alimentación a dicho molex o SATA.

La tecnología PWM requiere que, **si no detecta señal, los ventiladores y bombas funcionarán al 100%**, ya que como hemos dicho, siempre se entregan los **12 voltios**. Al producirse esta escena, el ventilador o la bomba puede sufrir daños en su motor.

Como último dato, *PWM* permite un rango más amplio de control de los ventiladores,  donde podremos evitar el límite de 5V impuesto por los tres pines. Sin embargo en las bombas de agua no es tan versátil ya que tienen un voltaje mínimo inamovible.

Cabe destacar que con *PWM* se consigue **reducir el consumo de energía y la sonoridad.**