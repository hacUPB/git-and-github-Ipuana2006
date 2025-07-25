# Como crear un Repositorio Remoto en GitHub y Sincronizarlo con un Repositorio Local

> Esta guía paso a paso te enseña cómo crear un repositorio remoto en GitHub y vincularlo con un repositorio local previamente inicializado con Git. Ideal para estudiantes, desarrolladores y equipos de trabajo que desean llevar un control profesional de versiones.

---

## Requisitos Previos

Antes de comenzar, asegúrate de tener:

-  Git instalado en tu computadora → [Instalar Git](https://git-scm.com/)
-  Una cuenta activa en [GitHub](https://github.com) (si no la tienes creala). 
-  Un repositorio local creado previamente (si no lo tienes, revisa la guía: *Cómo Crear un Repositorio Local con Git*)

---

### Paso 1: Crear un Repositorio Remoto en GitHub

1. Ingresa a tu cuenta de [GitHub](https://github.com).
2. En la esquina superior derecha, haz clic en el botón **`+` → "New repository"** o entra directamente a:  
    [https://github.com/new](https://github.com/new)
    ![alt text](<imagenes/Captura de pantalla 2025-07-25 143446.png>)
3. Rellena los siguientes campos:
   - **Repository name**: (Ej. `mi-proyecto`)
   - **Description**: (opcional pero recomendado)
   - **Visibility**: elige `Public` o `Private`
4. **Importante:** NO marques la opción `Initialize this repository with a README`, ya que enlazaremos uno local.
5. Haz clic en **`Create repository`**.
![alt text](<imagenes/Captura de pantalla 2025-07-25 144300.png>)
![alt text](<imagenes/Captura de pantalla 2025-07-25 144329.png>)
---

### Paso 2: Obtener la URL del Repositorio Remoto

Después de crear el repositorio, se te mostrará una URL como esta:
```bash
https://github.com/usuario/nombre-repositorio.git
```

Guarda esta URL, la necesitarás en el siguiente paso.

---

### Paso 3: Navegar al Repositorio Local

Abre la terminal y navega a la carpeta de tu repositorio local. Por ejemplo:

```bash
cd ~/Documentos/mi-proyecto
```
Si aún no lo creaste, puedes hacerlo así:

```bash
mkdir mi-proyecto
cd mi-proyecto
git init
```
### Paso 4: Enlazar el Repositorio Local al Repositorio Remoto
Con la terminal dentro de tu proyecto, escribe:

```bash
git remote add origin https://github.com/tu_usuario/mi-proyecto.git
```
Este comando le dice a Git que origin es el alias del repositorio remoto en GitHub.

### Paso 5: Subir tu Proyecto Local a GitHub
Antes de subir, asegúrate de tener al menos un commit:

```bash
git add .
git commit -m "Primer commit: estructura inicial"
```
Ahora, realiza el push (primer subida):

```bash
git push -u origin master
```
Si estás trabajando con la rama main (por defecto en versiones recientes de Git), usa:

```bash
git push -u origin main
```
Este comando empuja tu rama principal al repositorio remoto y establece la relación de seguimiento (-u).

### Paso 6: Verificar en GitHub
Ve al navegador y abre tu repositorio en GitHub.

Verifica que tus archivos aparezcan correctamente.

A partir de ahora, cualquier cambio local puede ser sincronizado con:

```bash
git push
```
Y si trabajas en equipo, puedes traer cambios con:

```bash
git pull
```
tambien sirve cuando tienes trabajo adelantado en el repositorio remoto y asi actualizar el repositorio local.
### Comandos Resumen

| Acción                         | Comando                                      |
|-------------------------------|----------------------------------------------|
| Inicializar repo local        | `git init`                                   |
| Enlazar con GitHub            | `git remote add origin <URL>`                |
| Ver remotos                   | `git remote -v`                              |
| Agregar archivos              | `git add .`                                  |
| Confirmar cambios (commit)    | `git commit -m "mensaje"`                    |
| Subir cambios a GitHub        | `git push -u origin main` *(o `master`)*     |
| Traer cambios desde GitHub    | `git pull`                                   |
| Ver estado del repo           | `git status`                                 |

## Conclusión
Sincronizar un repositorio local con GitHub es un paso fundamental para cualquier desarrollador o estudiante. Te permite:

- Tener un respaldo en la nube.

- Trabajar colaborativamente con control de versiones.

- Acceder a tu proyecto desde cualquier dispositivo.

- Mantener una documentación organizada y segura.

Dominar este flujo te brinda una base sólida para trabajar en proyectos personales y profesionales con buenas prácticas de desarrollo.


