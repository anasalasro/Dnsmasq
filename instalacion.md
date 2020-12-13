# Instalación de dnsmasq
## Para la instalación usaremos este comando
> apt install dnsmasq  

## Arranque y parada del servidor dnsmasq
El servicio dnsmasq, al igual que todos los servicios en Linux, dispone de scripts de arranque y parada en la carpeta /etc/init.d. Debemos ejecutarlos desde una consola de root.

>// Arrancar o reiniciar el servidor dnsmasq  
> /etc/init.d/dnsmasq restart  
>// Parar el servidor dnsmasq  
> /etc/init.d/dnsmasq stop  

## Configuración básica de dnsmasq  
**Editamos el fichero /etc/hosts**  

![Hosts](https://github.com/anasalasro/Dnsmasq/blob/main/imagenes/editamos-etc-hosts.png) 

**Editamos el fichero /etc/dnsmasq.conf**  

![Dnsmasq](https://github.com/anasalasro/Dnsmasq/blob/main/imagenes/fichero-etc-dnsmasqconf.png) 

**Editamos el fichero /etc/resolv.conf** 

![Resolv](https://github.com/anasalasro/Dnsmasq/blob/main/imagenes/editamos-etc-resolvconf.png) 

**Para finalizar reiniciamos es servicio**
> service dnsmasq restart
