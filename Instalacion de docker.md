Instalacion de docker
===

1. Ejecute este comando para descargar la versión estable actual de Docker Compose:

sudo apt-get update

2. Instale paquetes para permitir el uso de un repositorio sobre HTTPS:

sudo apt-get install \
apt-transport-https \
ca-certificates \
curl \
gnupg-agent \
software-properties-common

3. Agregue la clave GPG oficial de Docker:
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

4. Agregar los repositorios estables de Docker:
sudo add-apt-repository \
"deb [arch=amd64] https://download.docker.com/linux/ubuntu \
$(lsb_release -cs) \ stable"

5. Actualizar los paquetes relacionados con los repositorios del sistema:
sudo apt-get update

6. Instalar la versión para la comunidad, conocido como Docker CE.
sudo apt-get install docker-ce docker-ce-cli containerd.io


7. Verificar instalación de Docker
docker --version

referencia
===

https://jsgiraldoh.io/Blog/Instalar-Docker-Engine-en-Ubuntu/