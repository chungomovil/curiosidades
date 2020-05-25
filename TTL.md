### Tiempo de vida, *Time To Live (TTL)*

**TTL** es un concepto usado en redes de ordenadores para indicar **cuantos nodos puede pasar un paquete antes de ser descartado por la red o devuelto a su origen.**

El **TTL** forma parte de la *cabecera IP (Protocolo IP)* con un **tamaño de 8 bits.** El valor se inicializa en el **emisor** y tiene función de **ir descontando su contador una unidad según el datagrama IP viaje de un nodo a otro,** por lo que debe ser recalculado en cada salto.

Si dicho contador llega a cero, **descarta el paquete recibido y lo reenvía al emisor** en lugar de difundirlo. Este campo de la *cabecera IP* **impide la congestión** o sobrecargas de las líneas de transmisión, **el TTL se decrementa si también pasa un largo período en cola.** 

*En Internet este campo tiene un máximo arbitrario de 120 segundos, aunque depende del protocolo utilizado.*