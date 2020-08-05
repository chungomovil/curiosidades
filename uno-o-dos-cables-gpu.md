# En GPU con varios PCIe, ¿es mejor usar uno o dos cables de la fuente?



A la hora de proporcionarle alimentación a la **tarjeta gráfica** mediante los **cables PCIe** de la fuente de alimentación, nos pueden entrar las dudas en el caso de que la tarjeta gráfica necesite varios conectores: ¿deberías utilizar los **dos conectores de un mismo cable**, o es mejor utilizar **dos cables**? En este artículo vamos a proceder a analizar esta situación para sacarte de dudas.

Por norma general, la necesidad de utilizar dos cables distintos de la fuente de alimentación para dar servicio a tarjetas gráficas con varios conectores PCIe viene de antaño, cuando las fuentes de alimentación eran de cuando menos dudosa calidad -si bien es cierto que en la actualidad muchas siguen siéndolo- y utilizan muchos **raíles de +12V diferentes.** Cuando éste era el caso, si la gráfica requería más intensidad de corriente (Amperios) de lo que un solo raíl de +12V podía proporcionar, era de hecho necesario utilizar cables PCIe distintos.

![img](https://hardzone.es/app/uploads-hardzone.es/2017/01/Railes.jpg)

En la actualidad la mayoría de fuentes de alimentación de cierta calidad (hablamos de fuentes al menos Tier 1 o Tier 2) utilizan un único y potente raíl de +12V, por lo que el uso de cables PCIe diferentes es innecesario, con la excepción de que se utilicen cables de mala calidad, por supuesto. Técnicamente, si la fuente solo tiene un raíl de +12V, y siempre y cuando se cumplan los **requisitos de potencia e intensidad de la GPU**, no será necesario utilizar dos cables, y podrás darle a la gráfica la alimentación que necesita con un único cable con varios conectores PCIe.

### ¿En qué casos hay que usar varios cables para la gráfica?

Aunque la tarjeta gráfica funcione estando conectada con un único cable, hay ocasiones en las que es recomendable utilizar varios cables individuales, incluso aunque en un solo cable tengas varios conectores. Ten en cuenta que esto depende mucho de la marca, el modelo, el cableado y la edad de la fuente de alimentación, pero puede darse el caso de que por ejemplo tu gráfica tenga **Coil Whine**, y si eso sucede una de las primeras cosas que deberías probar es a conectarla con varios cables PCIe en lugar de con uno solo, ya que a veces el Coil Whine se produce por sobrecarga del cable precisamente.

![Conectar cable PCIe en fuente de alimentación](https://hardzone.es/app/uploads-hardzone.es/2019/11/psu-pcie.jpg)

También puede darse el caso de que aunque tu equipo funcione de manera normal, se te apague de repente cuando le exiges mucho gráficamente, es decir, cuando se pone la GPU al 100%. A veces esto sucede porque el cable está sobrecargado, y al igual que con el Coil Whine se soluciona simplemente conectando cada conector PCIe de la tarjeta gráfica con un cable PCIe de la fuente de manera individual. Esto es así porque en algunos casos, incluso aunque la fuente sea de calidad y tenga potencia de sobra, el cable no es de mala calidad, o podría estar **dañado o en mal estado**.

Finalmente, también es recomendable utilizar cables PCIe individuales de la fuente para dar servicio a la tarjeta gráfica en fuentes de alimentación de dudosa calidad (en caso de duda, usa dos cables) para evitar sobrecargas, así como en fuentes que tengan varios raíles de +12V.