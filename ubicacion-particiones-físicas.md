# Ubicación particiones físicas

### ¿Las particiones en los HDD y SSD influyen en el rendimiento? ¿están unidas físicamente?

Son dos grandes preguntas porque dependiendo de si hablamos de **HDD** o **SSD** hay una respuesta u otra. Comenzaremos por este último ya que es mucho más simple de responder y terminaremos con los HDD más en profundidad.

En un **SSD** una partición no influye en el rendimiento por la naturaleza del propio componente y sus **NAND Flash**. Al hacer una partición en un SSD lo único que hacemos es decirle al **MBR/GPT** cómo es la tabla de particiones y en que sectores y bloques comienza y termina cada una de ellas.

![particiones-ssd](https://hardzone.es/app/uploads-hardzone.es/2020/07/SSD-partition.jpg)



Como es lógico, los bloques se asignan para guardar un espacio predefinido según nuestras necesidades y debido a que **el controlador tarda el mismo tiempo en acceder a unos bloques u otros** no tendremos pérdida alguna de rendimiento.

Sobre la unión, normalmente un **SSD** reserva bloques enteros cuando se trata de particionar, de manera que se intenta no compartir dichos bloques entre dos particiones.

### ¿Por qué en un HDD esto no se cumple?

![disco-hdd](https://hardzone.es/app/uploads-hardzone.es/2013/10/Disco-duro-3D.jpg)



**Las partes exteriores de los platos giran a mayor velocidad de rotación** precisamente por su velocidad angular. Esto influye en un término conocido como **latencia rotacional**, la cual no es igual en todos los puntos del plato evidentemente.

Conforme más nos acerquemos al borde del mismo y más RPM tenga el motor y su eje, **menor latencia tendremos a la hora de leer los datos.** Esto influye directamente en el tiempo de búsqueda necesario para situar el cabezal en la pista concreta del plato, algo que ayuda al **NCQ** a calcular trayectorias más cortas.

![plato-hdd](https://hardzone.es/app/uploads-hardzone.es/2020/07/Velocidad-angular-HDD.png)

Por lo tanto, **un sistema operativo debería de estar situado en la periferia de un plato**, algo que **Windows y Linux consiguen de forma automática** siempre que no haya datos en el mismo antes de la instalación. Cuando se produce una partición, el cabezal marca principio y fin en el plato y a partir de ahí sigue escribiendo, por lo que hay una unión física entre particiones debido al magnetismo y material compartido.

**Pero, ¿qué ocurre si nuestro disco duro tiene varios platos?**

Lo ideal según los mecanismos de direccionamiento es que si la partición es factible en un plato, solo haya dos cabezales destinados para ella, dejando al resto sin trabajo, pero si esto no ocurre, la partición se hará en **distintos platos de modo simétrico**, por lo que la información se leerá y escribirá en todos ellos al mismo tiempo repartiendo la capacidad entre ellos.

