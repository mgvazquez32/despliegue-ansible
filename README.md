# Desafío 6 - Ansible: LAMP + WordPress en EC2

Este proyecto despliega automáticamente Apache, PHP, MariaDB y WordPress sobre una instancia EC2 Debian12 utilizando Ansible y roles separados por servicio.

Se utiliza una instancia Local Ubuntu para el despliegue y una instancia EC2 Debian12 en AWS para desplegar los servicios.

## 📁 Estructura del Proyecto

```bash
Desafio_6-Ansible/
├── inventory.ini
├── playbook.yaml
├── roles/
│   ├── apache/
│   │   ├── tasks/
│   │   │   └── main.yml
│   ├── php/
│   │   ├── tasks/
│   │   │   └── main.yml
│   ├── mysql/
│   │   ├── tasks/
│   │   │   └── main.yml
│   └── wordpress/
│       ├── tasks/
│       │   └── main.yml
