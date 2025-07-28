🔧 Requisitos previos
Tener una instancia corriendo Debian 12 (bookworm).

Conexión SSH válida (clave .pem si es AWS).

Instalar Ansible en tu máquina local:

bash
Copiar
Editar
pipx install --include-deps ansible
Clonar este repositorio:

bash
Copiar
Editar
git clone https://github.com/mgvazquez32/despliegue-ansible.git
cd despliegue-ansible/Desafio_6-Ansible
🗂 Estructura del proyecto
bash
Copiar
Editar
Desafio_6-Ansible/
├── inventory.ini
├── playbook.yaml
├── roles/
│   ├── apache/
│   ├── php/
│   ├── mysql/
│   └── wordpress/
└── pruebas/
    └── pruebabastion.png
📝 Configuración del inventario
El archivo inventory.ini debe contener la IP pública de tu instancia bajo un nombre de host:

ini
Copiar
Editar
[wordpress]
ec2-54-90-209-242.compute-1.amazonaws.com ansible_user=admin ansible_ssh_private_key_file=~/Descargas/Bastion.pem
Asegurate de reemplazar la IP y la ruta de tu clave según tu caso.

🚀 Ejecución del Playbook
Desde el directorio raíz del proyecto:

bash
Copiar
Editar
ansible-playbook -i inventory.ini playbook.yaml
Este Playbook ejecutará las siguientes tareas:

Instala y habilita Apache.

Instala PHP y módulos necesarios.

Instala y habilita MariaDB.

Descarga, extrae y configura WordPress.

📷 Evidencias
Se incluye una captura del resultado final en la carpeta pruebas:

pruebabastion.png


