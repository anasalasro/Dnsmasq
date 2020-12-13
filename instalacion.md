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
**Configuración como Caché DNS**  
Para que dnsmasq pueda ser un servidor caché DNS, es necesario que nuestro servidor tenga en el archivo de /etc/resolv.conf configurado al menos un servidor DNS externo. Normalmente los servidores DNS externos nos los proporciona el operador de telecomunicaciones que nos da servicio de Internet.  
Para que nuestro servidor utilice los DNS externos, debemos añadirlos en /etc/resolv.conf. En el caso de Telefónica, deberemos añadir en /etc/resolv.conf las siguientes líneas:  
>// Ejemplo: Utilización de los DNS externos de Telefónica  
>// Añadir en /etc/resolv.conf del servidor  
>nameserver 80.58.0.33  
>nameserver 80.58.32.97  

