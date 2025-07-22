# Desafío 6 - Ansible: LAMP + WordPress

Este repositorio contiene un proyecto modular con Ansible y Roles para desplegar automáticamente Apache, PHP, MySQL y WordPress en una instancia EC2 Ubuntu en AWS Academy.

## Estructura

- `inventory.ini`: define el host remoto.
- `playbook.yaml`: playbook principal.
- `roles/`: cada rol contiene sus tareas y variables.

## Requisitos

- Bastion de AWS Academy.
- Acceso a EC2 Ubuntu con clave PEM.
- Ansible instalado.

## Uso

```bash
ansible-playbook -i inventory.ini playbook.yaml
```

## Pruebas

Ver carpeta `pruebas/` con evidencias de ejecución exitosa.
