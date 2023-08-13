# Vortex86

La idea es recopilar todo el contenido interesante que tengamos sobre las MiniPCs con micro Vortex86SX.

También tenemos un grupo de Telegram para hablar de esto, lo pasamos por privado si querés entrar.

Si tenés alguna data para agregar o arreglar, podés abrir un _pull request_ o un _issue_ directamente! 

# Hardware

- Modelo: eBOX-2300SX
- CPU: MSTI PSX, que es equivalente a una Vortex86SX
- 128MB DDR2 RAM
- Salida VGA
- Puerto Ethernet 10/100 con auto MDI (no hace falta usar cable cruzado para conectar dos entre sí)
- 3 puertos USB
- Conector CompactFlash
- Se alimenta con 5V, consume menos de 1A, y es fanless

![Image](https://m.media-amazon.com/images/I/41fR1BKOhvL._AC_UF894,1000_QL80_.jpg)
![Versión con GPIO y puertos serie](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/EBOX_PC_2300_SX_internal.jpg/562px-EBOX_PC_2300_SX_internal.jpg)

![Block diagram](https://www.dmp.com.tw/tech/vortex86sx/img/Vortex86SX_block_diagram.gif)

## CPU
- Modelo: MSTI PSX 366MHz o a 300 MHz (depende de la placa)
- Es equivalente a una 486SX
- No tiene FPU, instrucciones de Pentium, ni extensiones tipo MMX
- El modelo de 300 se puede llegar a overclockear cambiandoo unas resistencias

- [Specs oficiales del SoC](https://www.dmp.com.tw/tech/vortex86sx/)

## Memorias CF
- [Memorias CF a buen precio](https://articulo.mercadolibre.com.ar/MLA-873109407-apacer-memoria-compact-flesh-cf5-32-gb-_JM?quantity=1)

## Problemas encontrados

## Modificaciones

- [Pines del cable de alimentación](https://www.youtube.com/watch?v=gUz2xTNYLwo&t=72s)
- [Armar conector de alimentación](https://www.youtube.com/watch?v=4KoLS5mJQUQ)
- [Bypass de cable de alimentación](mod_power_bypass.md)
- [Backup y modding de la BIOS](mod_bios.md)
- [Mod para agregar puerto serie RS232 o UART](mod_rs232.md)
- [Mod para agregar pines GPIO](mod_gpio.md)
- [Mod para agregar ESP8266 como bridge Wi-Fi](https://vintage2000.org/dos/serial_wifi_adapter)

# Software

## MS-DOS y FreeDOS
- [Jugar al Doom con dos Vortex conectadas entre sí (IPX)](dos_doom.md)
- [Conectar la Vortex a una red Ethernet/Internet](dos_ethernet.md)
- [Conectar MS-DOS a Mastodon](https://fabulous.systems/posts/2023/08/connecting-ms-dos-to-the-internet-and-the-fediverse/)
- [x86Launcher, un launcher gráfico para juegos y apps](https://github.com/megatron-uk/x86Launcher)ç
- [FrogFind, proxy y buscador de sitios viejos](http://frogfind.com/)
- [Drivers para dispositivos USB en DOS](https://www.bretjohnson.us/)
- [Gopherus, cliente de gopher para DOS](https://sourceforge.net/projects/gopherus/)
- [Juegos viejos de DOS](https://archive.org/details/DOSGamesCollection2015)

## Windows 3.1x y anteriores
- 

## Windows 95/98
- [Parche para CPUs modernas, no hace nada en las Vortex](https://github.com/JHRobotics/patcher9x)
- [Protoweb, una máquina del tiempo de internet](https://protoweb.org/)

## Linux
- [X-linux, la distro "oficial" de los fabricantes (ya tiene un kernel viejito)](http://www.dmp.com.tw/tech/os-xlinux/xlinux-manual-5.7.htm)
- [Compilar Linux para 486](https://ocawesome101.github.io/486-linux.html)

## Windows CE
- [Imagen CE 5.0 demo oficial (con X-Linux y FreeDOS también)](http://www.dmp.com.tw/tech/vortex86sx/demo/070529.GHO)

## Otros: 
- OS/2: Crashea antes de terminar de bootear
- Memtest: corre bien hasta la versión 4.1
