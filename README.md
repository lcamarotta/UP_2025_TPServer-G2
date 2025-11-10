# COMPUTACIÓN APLICADA - Trabajo Práctico Integrador

**Universidad de Palermo - Facultad de Ingeniería**

---

## Integrantes Grupo 2

* Camarotta, Lucas
* Flores, Valentin
* Armendariz, Iñaki

---

## Descripción

Este repositorio contiene la resolución del Trabajo Práctico Integrador de la materia **Computación Aplicada**.

El proyecto consistió en la configuración completa de un servidor **GNU/Linux Debian** partiendo de una máquina virtual preinstalada. Los objetivos principales cubiertos fueron:

1.  **Configuración del Entorno:** Restablecimiento de la contraseña de `root` y configuración del hostname `TPServer`.
2.  **Instalación de Servicios:**
    * **SSH:** Configuración de `openssh-server` para permitir el acceso por clave pública/privada.
    * **Servidor Web:** Instalación de **Apache2** con soporte **PHP**.
    * **Base de Datos:** Instalación de **MariaDB** y carga de un script SQL inicial.
3.  **Configuración de Red:** Establecimiento de una dirección IP estática en el servidor.
4.  **Almacenamiento:**
    * Adición de un nuevo disco de 10 GB.
    * Creación y formateo de dos particiones: `/www_dir` (3 GB) y `/backup_dir` (6 GB).
    * Configuración del montaje automático de las nuevas particiones en `/etc/fstab`.
    * Reconfiguración de Apache para servir el sitio desde el nuevo directorio `/www_dir`.
5.  **Script de Backup:**
    * Desarrollo del script `backup_full.sh` para automatizar copias de seguridad.
    * Programación de tareas con `cron` para ejecuciones automáticas.

---

## Informe Detallado

El informe completo con el paso a paso, los comandos ejecutados y las capturas de pantalla de cada consigna se encuentra en el archivo **`TPIntegaror_Grupo2.pdf`**, incluido en este repositorio.

---

## Diagrama Topológico

A continuación, se presenta el diagrama topológico de la infraestructura implementada, según lo solicitado en los entregables.

<p align="center">
  <img width="701" height="501" alt="TPServer drawio" src="https://github.com/user-attachments/assets/ad897c26-ff3d-43aa-8b76-546259d0006b" />
</p>

---

## Contenido del Repositorio

* `README.md`: Este archivo.
* `TPIntegaror_Grupo2.pdf`: Informe detallado del trabajo práctico.
* `TPServer.drawio.png`: Diagrama topológico de la red.
* `root.tar.gz`: Directorio `/root` comprimido.
* `etc.tar.gz`: Directorio `/etc` comprimido.
* `opt.tar.gz`: Directorio `/opt` comprimido.
* `www_dir.tar.gz`: Directorio `/www_dir` comprimido.
* `backup_dir.tar.gz`: Directorio `/backup_dir` comprimido.
* `var_part_*`: Directorio `/var` comprimido y dividido en partes.
