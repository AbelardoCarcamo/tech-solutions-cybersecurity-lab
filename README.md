# Enterprise Cybersecurity Lab – Tech.Solutions

Este proyecto consiste en un **laboratorio de infraestructura empresarial** desplegado en **Oracle Cloud Infrastructure (OCI)**, diseñado para simular un entorno corporativo real con servicios de directorio activo, gestión de identidades, automatización de usuarios y monitoreo de seguridad.

El objetivo del laboratorio es **replicar una arquitectura empresarial real** para practicar:

- Administración de sistemas
- Gestión centralizada de identidades
- Automatización de usuarios
- Monitoreo de eventos de seguridad
- Arquitectura Cloud

---

# Autores

**Abelardo Cárcamo**  
**Chester Ferrer**

---

# ☁️ Infraestructura del laboratorio

Toda la infraestructura del proyecto se encuentra desplegada en **Oracle Cloud Infrastructure (OCI)**.

Este laboratorio busca simular una **infraestructura empresarial típica**, donde los servicios críticos están centralizados y gestionados desde un controlador de dominio.

## Componentes implementados

- Active Directory Domain Controller
- Gestión de usuarios mediante ManageEngine
- Plataforma de monitoreo con Splunk
- Acceso remoto mediante RDP
- Automatización de creación de usuarios

---

# Active Directory Domain Controller

Se implementó un controlador de dominio utilizando **Windows Server**.

## Dominio configurado

**tech.solutions**

El servidor cumple las siguientes funciones:

- **Controlador de dominio (Domain Controller)**
- **Servidor de autenticación**
- **Administrador central de identidades**

Este componente representa el **núcleo de la infraestructura del laboratorio**.

---

# Gestión de usuarios

La administración de usuarios se realiza mediante **ManageEngine ADManager Plus**, una plataforma que permite gestionar cuentas de Active Directory desde una interfaz web.

## Funcionalidades utilizadas

- Creación de usuarios
- Administración centralizada del directorio
- Automatización de procesos de gestión de identidades

---

# Usuarios creados en el dominio

## Usuarios administrativos

Se crearon dos cuentas administrativas para la gestión del entorno:

- **chester**
- **Abcarcamo**

Como práctica de seguridad, el usuario predeterminado **Administrator** fue deshabilitado para evitar el uso de cuentas administrativas por defecto.

---

# Usuarios de prueba

Para validar el funcionamiento del sistema de gestión de usuarios, se crearon dos cuentas de prueba desde ManageEngine:

- **Prueba**
- **Prueba_1**

Estas cuentas se utilizan para pruebas de administración y automatización.

---

# Automatización de creación de usuarios

Uno de los objetivos del laboratorio es implementar **automatización en la gestión de identidades**.

ManageEngine ADManager Plus permite crear múltiples usuarios mediante la importación de archivos **CSV**.

## Flujo del proceso

1. Crear un archivo CSV con la información de los usuarios
2. Importar el archivo dentro del módulo de automatización de ADManager
3. Ejecutar la tarea automatizada para crear las cuentas en Active Directory

Este proceso simula el **provisionamiento masivo de usuarios en entornos empresariales**, donde las cuentas suelen generarse automáticamente a partir de sistemas de recursos humanos.

---

# Acceso remoto al servidor

El acceso al servidor se realiza mediante **Remote Desktop Protocol (RDP)**.

Para iniciar sesión dentro del dominio se debe utilizar el formato:

tech.solutions\Abcarcamo

Esto indica que la autenticación se realiza contra el dominio **tech.solutions**.

---

# Sistema de monitoreo (SIEM)

Para el monitoreo de eventos del sistema se instaló **Splunk Enterprise**.

Splunk permitirá:

- Centralizar logs del sistema
- Monitorear eventos de seguridad
- Detectar comportamientos anómalos
- Simular operaciones de **Blue Team**

---

# Componentes en desarrollo

El laboratorio continuará expandiéndose con nuevos servicios para simular una infraestructura empresarial más completa.

## Próximos componentes

- Configuración de **DHCP Server**
- Implementación de red privada con **Tailscale**
- Instalación de **bases de datos empresariales**
- Integración completa de logs en Splunk
- Simulación de escenarios de seguridad

---

# Objetivo del proyecto

El objetivo de este laboratorio es **recrear una infraestructura empresarial funcional** para practicar:

- Administración de sistemas
- Gestión de identidades
- Monitoreo de seguridad
- Arquitectura Cloud
- Automatización de procesos IT

---

# Uso educativo

Este proyecto fue desarrollado con fines **educativos y de aprendizaje en infraestructura empresarial, cloud computing y ciberseguridad**.
