# ansible_siguca [![Build Status](https://travis-ci.org/fede2cr/ansible_siguca.svg?branch=master)](https://travis-ci.org/fede2cr/ansible_siguca)

Recetas de ansible para instalar una unidad de marcado RFID para el software SIGUCA, utilizando la herramienta automatizada Ansible

## Requerimientos

Para seguir este tutorial necesita una Raspberry Pi3, el instalador de Rasbpian o Noobs, un lector RFID serial, y una pantalla de 7 pulgadas para Raspberry Pi.

## Uso

Con ansible instalado en el equipo del operador, conectamos una Raspberry Pi con Rasbpian recién instalado, editamos ``inventory/hosts`` para definir el IP de la Pi, y luego ejecutamos desde el equipo del operador:

```bash
git clone https://github.com/fede2cr/ansible_siguca.git
cd ansible_siguca
ansible_playbook 01-upgrade.yml 02-preparacion_pi.yml
```

Una vez completado esto, ya debería tener:
- [ ] Script de arranque para la interfaz gráfica de Siguca
- [ ] Instalación de base de datos mongodb, y aplicación de Siguca
- [ ] Capacidad de definir el servidor de aplicación de Siguca, para enviar los datos de marca
