# Composición del núcleo de una tarjeta gráfica

Una **tarjeta gráfica posee núcleo o encapsulado**. Este núcleo principal con millones de transistores **se divide a su vez en pequeños núcleos**, en el que cada **conjunto de estos núcleos está diseñado y optimizado para hacer una tarea específica**.

A continuación veremos como se dividen y que función realizan:

Partimos de que cada GPU posee múltiples **GPC (Graphics Processing Cluster)**, que no es más que el contenedor que agrupa los núcleos que realmente nos importan analizar.

![gpc](E:\Documentos\curiosidades\markdown\images\gpc.jpg)

Cada **GPC** está formado por varios **SM (Streaming Multiprocessors)**, **ROPs (Render Output Units)**, **TMUs (Texture Mapping Units)** y en la RTX además vienen integrados los **RT Cores y Tensor Cores**.



### SM o Stream MultiProcessors

Los **SM** son agrupaciones de Cuda Cores, normalmente cada SM tiene 64 Cuda Cores.

![sm](E:\Documentos\curiosidades\markdown\images\sm.jpg)

Los **Cuda Cores** son los encargados de **realizar cálculos matemáticos y multiplicación de matrices** para ubicar los objetos en la escena, es decir, **rotan, escalan y trasladan los objetos** para que se **muestren en pantalla como se desea** en una determinada escena.

![cudacores](E:\Documentos\curiosidades\markdown\images\cudacores.jpg)



### TMUs o Texture Mapping Units

Los **TMUs** son los núcleos especializados en **poner las texturas** sobre las matrices y puntos calculados anteriormente. **Este proceso es similar a poner una imagen (textura) sobre las matrices.**

![tmus](E:\Documentos\curiosidades\markdown\images\tmus.jpg)

**En la siguiente imagen se aprecia un objeto que aun no posee texturas:**

<img src="E:\Documentos\curiosidades\markdown\images\sin-textura.gif" style="zoom:67%;" />

**Y ahora se muestra una imagen con texturas:**

<img src="E:\Documentos\curiosidades\markdown\images\con-textura.gif" style="zoom:67%;" />



### ROPs o Render OutPut Units

Por otra parte los **ROPS**, se encargan de transformar toda la información anterior (matrices y texturas) a píxeles para que estos sean mostrados en pantalla.

![rops](E:\Documentos\curiosidades\markdown\images\rops.jpg)



### RT Cores

De forma resumida, **los RT Cores son los encargados de calcular la iluminación de la escena en tiempo real.** Es decir, en el momento de realizar el RayTracing los **Cuda Cores le envían la información de los polígonos y los rayos de luz a calcular a los RT Cores.** **Éstos hacen los cálculos necesarios para saber de que forma se debe iluminar cada polígono** y se lo envían de vuelta a los Cuda Cores. Debido a que es su única tarea, estos núcleos son extremadamente rápidos ejecutando su trabajo. Nvidia en la seria RTX 2000 añadió un RT Core por cada SM.

![rtcore](E:\Documentos\curiosidades\markdown\images\rtcore.jpg)



### Tensor Cores

**Los Tensor Cores núcleos son los encargados de la inteligencia artificial y Deep Learning.** En un principio solo tenían utilidad en el sector profesional y automovilístico. Pero con la llegada de **DLSS** a los videojuegos se les comenzó a dar uso.

**En el campo de los videojuegos estos núcleos reescalan imágenes desde resoluciones más bajas sin apenas perder calidad de imagen** gracias a la inteligencia artificial. Con DLSS 2.0 incluso el reescalado aumenta la nitidez con respecto a jugar a una resolución nativa. Es decir que se vería mejor y con más detalles una imagen reescalada desde 720p a 4K que una imagen en 4K nativa.

![tensorcore](E:\Documentos\curiosidades\markdown\images\tensorcore.jpg)