# Uso de la Consola y Control de Versiones con Git

Este documento resume los conceptos aprendidos sobre el uso de la consola para navegar, crear archivos y directorios, así como los comandos básicos utilizados. También se incluye una introducción al control de versiones con Git, incluyendo cómo inicializar un repositorio y realizar commits.

---

## Navegación en la Consola

La consola o terminal permite interactuar directamente con el sistema operativo mediante comandos. Es una herramienta poderosa para desarrolladores.

### Principales comandos de navegación:

| Comando              | Descripción                                      |
|----------------------|--------------------------------------------------|
| `pwd`                | Muestra el directorio actual                     |
| `ls`                 | Lista los archivos y carpetas del directorio     |
| `cd <carpeta>`       | Cambia al directorio especificado                |
| `cd ..`              | Sube un nivel en la jerarquía de carpetas        |
| `clear`              | Limpia la consola                                |

---

## Creación de Archivos y Directorios

### Comandos esenciales:

| Comando                    | Descripción                                     |
|----------------------------|-------------------------------------------------|
| `mkdir <nombre>`           | Crea una nueva carpeta                          |
| `touch <archivo>`          | Crea un nuevo archivo vacío                     |
| `vim   <archivo>`           | Abre un editor de texto dentro de la terminal  |
| `rm <archivo>`             | Elimina un archivo                              |
| `rmdir <carpeta>`          | Elimina una carpeta vacía                       |

---

# Introducción al Control de Versiones con Git

Git es un sistema de control de versiones distribuido ampliamente utilizado por desarrolladores. Permite llevar un historial de los cambios en los archivos de un proyecto, facilita el trabajo colaborativo y ayuda a mantener un flujo de trabajo organizado y seguro.

---

## ¿Qué es el Control de Versiones?

El control de versiones permite:

- Registrar todos los cambios realizados en un proyecto.
- Volver a versiones anteriores si ocurre un error.
- Trabajar en equipo sin sobrescribir el trabajo de otros.
- Mantener un historial claro y detallado del desarrollo.

---

## ¿Qué es Git?

Git es una herramienta de control de versiones que se ejecuta desde la consola. Permite crear repositorios donde se almacena el historial de cambios de un proyecto.

---

## Primeros Pasos con Git

### 1. Inicializar un Repositorio

Para comenzar a usar Git en una carpeta de tu proyecto, navega a esa carpeta con la consola y ejecuta:

```bash
git init # para initializar un repositorio.

```

### 2. Crear o Modificar Archivos
Puedes usar cualquier editor para crear archivos:

```bash
touch index.py 
vim script.js

```

### 3. Ver el Estado del Repositorio
Este comando muestra qué archivos han sido modificados, añadidos o eliminados:

```bash
git status

```
### 4. Añadir Archivos al Área de Staging
Antes de confirmar los cambios, debes indicarle a Git qué archivos quieres incluir en el commit:

```bash
git add archivo.txt     # Añadir un archivo específico
git add .               # Añadir todos los archivos modificados

```
### 5. Hacer un Commit
Un commit guarda un conjunto de cambios con un mensaje descriptivo. Es como tomar una "foto" del estado actual del proyecto:

```bash
git commit -m "Mensaje que describa los cambios"
```
Ejemplo:

```bash
git commit -m "Agregué estructura base del HTML"

```
6. Ver el Historial de Cambios
Para ver todos los commits realizados hasta el momento:

```bash
git log

```

## Conclusión
Git es una herramienta esencial en el desarrollo de software. Dominar sus comandos básicos permite mantener tus proyectos organizados, seguros y colaborativos desde el inicio. El uso combinado de la consola y Git te proporciona control total sobre tu entorno de desarrollo.

