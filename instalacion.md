# Instalacion de dnsmasq
## Para la instalación usaremos este comando
> apt install dnsmasq  

## Arranque y parada del servidor dnsmasq
El servicio dnsmasq, al igual que todos los servicios en Linux, dispone de scripts de arranque y parada en la carpeta /etc/init.d. Debemos ejecutarlos desde una consola de root.

>// Arrancar o reiniciar el servidor dnsmasq  
> /etc/init.d/dnsmasq restart  
>// Parar el servidor dnsmasq  
> /etc/init.d/dnsmasq stop  

Para un arranque automático del servicio al iniciar el servidor, debemos crear los enlaces simbólicos correspondientes con el comando update-rc.d
