# Conectar la Vortex a una red Ethernet/Internet

- [Descargar y extraer el packet driver de la placa de red](http://www.dmp.com.tw/tech/vortex86sx/dos/pktdrv.zip)
- [Descargar y extraer el stack TCP y otras utilidades](http://mirror.vintage2000.org/oldnet.zip)
- Conectar el cable de red desde la Vortex a una red ethernet
- Copiar los archivos de ambos paquetes al disco o pendrive de la Vortex
- Ir a la carpeta donde se extrajeron los archivos (en este caso `C:\oldnet\`)
- Ejecutar `r6040pd 0x60`
- Ejecutar `echo PACKETINT 0x60 > mtcp.cfg`
- Ejecutar `set MTCPCFG=C:\oldnet\mtcp.cfg`
- Ejecutar `dhcp`

Si funciona todo bien la Vortex debería tener su propia IP, y se deberían poder usar las distintas utilidades provistas: `ping, htget, ircjr, telnet, microweb, ...` y cualquier otra cosa que use el stack mTCP.