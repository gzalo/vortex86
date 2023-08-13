# Agregar pines GPIO

En el caso de tener la versión de la placa tiene los pines de GPIO disponibles (en el frente, al lado de la tarjeta CF) en muchos casos no se puede usar directamente porque le faltan algunos componentes: RP6 a RP11 Y F4. Los mismos son usados como una protección básica (limitan la corriente) por si se llega a hacer un cortocircuito entre pines o a masa: 

- RP6 a RP11 pueden ser reemplazados por packs de resistencias de 100 o 150 ohms, sacados de otros equipos.
- Si es necesario usar el pin 1 como +5V, se puede soldarun polyfuse de 500 mA o similar en F4.

En el caso de que no aparezcan los puertos GPIO para configurar en la BIOS, puede que sea necesario modificar la BIOS para que soporte configurarlos desde su menú, y luego habilitarlos. [Ver más información sobre esa modificación](mod_bios.md)

Hay 24 pines GPIO expuestos, y algunos de los mismos pueden ser usados con el periférico SPI interno, pero esto aún no se probó:
- SPICS GPIO30
- SPIDI GPIO33
- SPICLK GPIO31
- SPIDO GPIO32

[Para programar software que use los pines se puede usar como referencia este documento](http://www.dmp.com.tw/tech/DMP_Vortex86_Series_Software_Programming_Reference_091216.pdf). Es relativamente sencillo, un registro de I/O se puede usar para definir la dirección de cada pin, y con otro se puede leer y escribir su valor. Se puede usar las funciones `outportb` e `inportb` de los distintos lenguajes de programación de esa época.
