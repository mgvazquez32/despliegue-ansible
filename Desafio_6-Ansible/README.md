# Desafío 6 - Ansible: LAMP + WordPress

Proyecto modular con Ansible y Roles para desplegar automáticamente Apache, PHP, MySQL y WordPress en una instancia EC2 Ubuntu.

## Estructura

- `inventory.ini`: define el host remoto.
- `playbook.yaml`: playbook principal.
- `roles/`: cada rol contiene sus tareas y variables.

## Requisitos

- Bastion de AWS Academy.
- Ubuntu Local con clave PEM.
- Ansible instalado.

## Uso

```bash
ansible-playbook -i inventory.ini playbook.yaml
```

## Pruebas

Ver carpeta `pruebas/` con evidencias de ejecución exitosa.
