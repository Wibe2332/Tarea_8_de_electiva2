Automatización con Ansible y Docker - Práctica Electiva 2
Descripción
Este proyecto automatiza la configuración de 5 servidores Ubuntu usando Docker y Ansible. Se creó una imagen base de Ubuntu con SSH habilitado y un usuario ansible para la administración. Luego, con Docker Compose, se levantaron 5 contenedores como servidores.

Ansible se usa para:

Actualizar los paquetes del sistema operativo

Crear el usuario itla en cada servidor

Crear la carpeta /home/itla/app

Crear el archivo hola.txt dentro de la carpeta con un mensaje

Instalar las aplicaciones cowsay y htop

Configurar el PATH del usuario itla para usar correctamente cowsay

Archivos principales
Dockerfile: Imagen base de Ubuntu con SSH y usuario ansible

docker-compose.yml: Levanta 5 servidores Ubuntu

inventario.ini: Lista los servidores y puertos SSH para Ansible

ansible.cfg: Configuración de Ansible para usar el inventario y evitar advertencias SSH

playbook.yml: Playbook de Ansible que realiza todas las tareas de configuración
