Practica 1 Instalacion de Webmin (1Pts )

Instala webmin
Muestre las Opciones de adminsitracion que se pueden ejecutar via Webmin (Administración de usuarios: Crear, y eliminar una cuenta de usuario, Gestión de servicios: Iniciar, detener y reiniciar servicio del sistema (Ej SSH). Configuración de red: Configurar una IP estatica en interfaces de red, Administración de software: actualizar  Instalar,y eliminar Alguna herramienta.Gestión de archivos y directorios: Explorar, editar un archivo y eliminarlo. Monitorización del sistema: Supervisar el rendimiento del sistema,(Memoria, Procesador Armacenamiento)
Practica 2 Desplieque de una VM con terraform en digital Ocean(1Pts)

Proceda a instalar Terraform en la VM Server https://developer.hashicorp.com/terraform/install
desplegar una VM usando terraform en una VM de digital ocean con las siguientes spec.
image: ubuntu-22-04-x64
name:OS3vm
region:nyc1
size:s-1vcpu-1gb
ssh_key [llavePublicaDeTuServerAnsible]
Documentacion AQUI

Validar la creacion de la VM ingresando via SSH y tambien por el portal web de digital Ocean para validar que el despliegue se realzio de forma correcta.

Practica 3: Instalación de Ansible (1pts)

Instalar ansible en la VM-Server (que funionara como ansible controller) junto a todas sus dependencias
Configurar ambos equipos clientes (la VM de digital ocean y la VM de windows) para que sean compatibles con el ansible controller
Crea un usuario llamado ansible con permisos de administrador (en el caso de windows y sudoers en el caso de linux) 
El usuario ansible puede iniciar sesión en ansible1 usando ssh, basándose en par de llaves ssh sin contraseña.
Crear un inventario de ansible (/etc/ansible/host) y crear un grupo llamado [win] para la pc de windows y uno llamado [linux] para la VM de linux
pruebe la conexion a ambos host utilizando el modulo ping
Practica 4: Comandos Ad-Hoc (1Pts)

Utilizando el modulo win_copy utilize un comando ad-hoc que copie un archivo txt ubicado en el escritorio de la maquina ansible2 a la carpeta de documentos
Utilizando el modulo reboot utilize un comando ad-hoc que reinicie la VM ansible 1
Practica 5: Playbooks (1Pts)

Crear un playbook para instalar la aplicacion notepad++ en la maquina ansible2 (Windows)
Crea un playbook en la maquina ansible1 (linux) para que instale NGINX e inicie el servicio
