# Practica-IniciacionVirtualizacion
# Instalación docker en ubuntu 24.04
### José Carlos Goméz-Lobo Ramírez


## 1.Nos aseguramos de que el sistema este actualizado  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/1.png)  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/2.png)
Actualizo los repositorios  
sudo apt update && sudo apt upgrade -y  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/3.png)  
Instalo dependencias  
sudo apt install ca-certificates curl gnupg lsb-release -y  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/4.png)  
Añado el repositorio de Docker e instalo Docker Desktop  
curl -fsSL https://get.docker.com | sudo sh sudo apt install docker-desktop -y  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/5.png)  
sudo apt update && sudo apt upgrade -y  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/6.png)  
sudo apt install docker-desktop -y  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/7.png)  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/8.png)  
Verifico que Docker funciona correctamente
docker --version  
docker run hello-world  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/9.png)  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/10.png)  
Busco imágenes disponibles
docker search nginx  
docker search tomcat  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/12.png)  
Descargo e inicio contenedores
docker run -d -p 8080:80 --name webserver nginx  
docker run -d -p 8081:8080 --name appserver tomcat  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/13.png)  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/14.png)
Verifico contenedores activos
docker ps  
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/15.png)
![Pagina principal](https://raw.githubusercontent.com/JosecarlosGlr/Practica-Iniciaci-nVirtualizaci-n/refs/heads/main/16.png)
Navegador en ambos servidores

##Descripción de requerimientos minimos

Para desplegar una aplicación web se necesita un hardware básico con suficiente CPU, RAM y espacio en disco, junto con un sistema operativo y un servidor web adecuados. La infraestructura de red debe estar bien configurada para permitir el acceso mediante IP, puertos y, si procede, DNS. También es necesario ajustar la configuración del servidor web y de la aplicación para asegurar su correcto funcionamiento. Además, deben aplicarse medidas de seguridad y mantenimiento como actualizaciones, uso de HTTPS, cortafuegos y copias de seguridad.

## Conclusiones

En este trabajo se ha aprendido a instalar y configurar Ubuntu en VirtualBox, así como a instalar y utilizar Docker, comprendiendo los comandos básicos para crear y ejecutar contenedores. Además, se ha analizado qué se necesita para desplegar una aplicación web, incluyendo hardware, software, infraestructura de red, configuración del servidor y medidas de seguridad. Todo ello permite entender cómo preparar un entorno seguro y funcional, y proporciona una base sólida para gestionar aplicaciones web de manera eficiente.


