# ansible_mysql_exporter

Repo con roles en ansible para configurar mysql exporter de Prometheus para recoger metricas de bases de datos.

Testeado con Vagrant + qemu + ubuntu_2204 + ansible_2.10

---

### Descripción
La idea del proyecto es automatizar vía ansible la instalación/configuración de una base de datos con mariadb y configurar mysql_exporter para pruebas de laboratorio, el repo cuenta con 2 roles:

- mariadb
- mysql_exporter

### Dependencias

* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)
* [Vagrant](https://developer.hashicorp.com/vagrant/install) - opcional

### Uso
```
git clone https://github.com/pgraffigna/ansible_role_mysql_exporter.git
cd ansible_role_mysql_exporter
ansible-playbook main.yml
```

### Extras
* Archivo de configuración (Vagrantfile) para desplegar una VM descartable con ubuntu-22.04 con libvirt como hipervisor.
* Archivos docker-compose para desplegar un entorno de base de datos con mysql o postgres + pgadmin4.
