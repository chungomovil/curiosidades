# Nvidia Encoder o NVENC

**Nvidia Encoder o abreviado (NVENC)** no es más que una **codificación de vídeo** que se realiza en la GPU liberando así a la CPU de esta intensiva carga. A partir de la generación Pascal (GTX 1000) se utilizan núcleos de la gráfica dedicados a esta tarea únicamente.

En la siguiente imagen se pueden apreciar las diferencias:

<img src="https://www.noticias3d.com/imagenes/noticias/201902/2w554.png" alt="obs-nvenc" style="zoom:150%;" />



Las RTX son hasta un 15% más eficientes debido a que necesitan un 15% menos de bitrate para conseguir una imagen de la misma calidad que la serie anterior (*Pascal*) cuando se hace stream en H.264 gracias a la mejora por hardware dedicado NVENC de las gráficas *Turing (RTX 2000).*

Esto significa que las GPUs GeForce RTX pueden stremear con una calidad de imagen superior en comparación con x264 Fast y a la par con x264 Medium.

<img src="https://www.noticias3d.com/imagenes/noticias/201902/75567.png" alt="bitrate" style="zoom:150%;" />

![comparacion](https://www.noticias3d.com/imagenes/noticias/201902/67767.png)

![comparacion2](https://www.noticias3d.com/imagenes/noticias/201902/8685769.png)