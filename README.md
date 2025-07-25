[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/cyLOSpir)
# Unidad No. 1 - Git y GitHub
## Información del estudiante  
Nombre del estudiante:  
Id.:  
---
# Evaluación
### descripcion del contenido del repositorio 
# Uso de la Consola y Git para el Control de Versiones

## Descripción

Este repositorio contiene una guía práctica y paso a paso sobre cómo utilizar la consola (terminal) del sistema operativo, cómo utilizar Git para el control de versiones, y cómo crear, gestionar y sincronizar repositorios locales y remotos, especialmente usando GitHub.

Está dirigido a estudiantes, principiantes en desarrollo de software o cualquier persona interesada en aprender buenas prácticas para la gestión de proyectos con Git.

---

## Contenido del Repositorio

- `uso_consola.md`: Introducción básica al uso de la terminal de comandos.
- `repositorio_local.md`: Cómo inicializar un repositorio local con Git.
- `repositorio_remoto.md`: Cómo crear un repositorio en GitHub y enlazarlo con el repositorio local.
- `README.md`: Descripción general del proyecto.
- Ejemplos prácticos y comandos útiles de Git.
- Tablas resumen para facilitar el aprendizaje y consulta rápida.

---

## Cómo Clonar y Ejecutar este Proyecto

Sigue estos pasos para clonar este repositorio en tu máquina local y comenzar a utilizarlo:

---

### 1. Clonar el Repositorio
Antes de clonar el repositorio remoto asegurate de que sea en una carpeta la cual te sea facil de ingresar. todo eso lo puiedes hacer desde la terminal de tu computadora. tambeien nececitaras instalar git en tu computadora( [Instalar Git](https://git-scm.com/) ).

Abre tu terminal y ejecuta el siguiente comando:

```bash
git clone https://github.com/tu_usuario/nombre-del-repositorio.git
```
la URL es la del repositorio remoto que deseas clonar.
Reemplaza tu_usuario y nombre-del-repositorio con la URL real de este proyecto.

### 2. Acceder a la Carpeta del Proyecto
```bash
cd nombre-del-repositorio
```
### 3. Explorar el Contenido
Dentro del proyecto encontrarás archivos .md que explican paso a paso cómo:

- Usar la terminal o consola del sistema.

- Crear y trabajar con un repositorio local con Git.

- Enlazar y sincronizar el repositorio con GitHub.

- Usar comandos útiles y buenas prácticas de control de versiones.

Puedes abrir los archivos .md con cualquier editor de texto o visualizador de Markdown como Visual Studio Code.

### 4. Personalizar y Probar
Este proyecto es educativo, así que puedes:

Modificar los archivos .md para adaptarlos a tus apuntes o presentaciones.

Probar los comandos de Git en tu propio repositorio local.

Hacer tus propios commits y experimentar con GitHub.
## Tabla de Contenido

Haz clic en cualquiera de los documentos para acceder a la guía correspondiente:

| Tema                                      | Archivo Markdown |
|------------------------------------------|------------------|
| Uso básico de la consola               | [uso_consola.md](docs/uso_consola.md) |
| Crear un repositorio local con Git     | [repositorio_local.md](docs/repositorio_local.md) |
| Sincronizar con un repositorio remoto  | [repositorio_remoto.md](docs/repositorio_remoto.md) |


#### **Descripción de la Actividad:**

El objetivo de esta actividad es crear y estructurar un proyecto de programación utilizando Git y GitHub. Aunque el código fuente será un componente mínimo, el enfoque estará en la organización del proyecto y la documentación de lo aprendido sobre los siguientes temas:

1. Uso de la consola para navegar entre directorios, crear directorios y archivos.
2. Creación de repositorios locales usando comandos de Git.
3. Creación de repositorio remoto en GitHub y sincronización con el repositorio local.

**Instrucciones:**

1. **Crea la estructura del proyecto:**
    - Clona el repositorio de la evaluación.
    - De ahora en adelante seguirás trabajando en tu repositorio local.
    - Ubícate en el directorio raíz llamado `prog-Eval_Template`.
    - Dentro de este directorio, crea las siguientes carpetas:
        - `src`: para almacenar el código fuente.
        - `docs`: para guardar la documentación.
        - `images`: para imágenes relacionadas con el proyecto.
2. **Código fuente:**
    - En la carpeta `src`, crea un script en Python (ej. script.py) con el siguiente código:
        
        ```python
        # Programa para calcular el promedio de una lista de números
        
        print("Bienvenido al programa de cálculo de promedios.")
        print("Ingresa números uno por uno. Escribe 'salir' para terminar.")
        
        # Lista para almacenar los números
        numeros = []
        
        while True:
            entrada = input("Ingresa un número (o escribe 'salir'): ")
            
            if entrada.lower() == 'salir':
                break  # Salir del bucle si el usuario escribe 'salir'
            
            try:
                # Convertir la entrada a número
                numero = float(entrada)
                numeros.append(numero)
            except ValueError:
                print("Por favor, ingresa un número válido.")
                continue
        
        # Verificar si hay números en la lista antes de calcular el promedio
        if len(numeros) > 0:
            promedio = sum(numeros) / len(numeros)
            print(f"El promedio de los números ingresados es: {promedio:.2f}")
        else:
            print("No ingresaste ningún número.")
        
        ```
        
    - Este código es solo un ejemplo básico para incluir un archivo funcional en el proyecto.
3. **Archivo .gitignore:**
    
    Investiga qué es un archivo `.gitignore` y cuál es su función dentro de un proyecto de programación. Crea el archivo `.gitignore` y guárdalo en a tu repositorio. Ahora, según la consulta que hiciste, escribe en él, los nombres de archivos y carpetas que quieres ignorar. Pregunta al profesor en caso de dudas.
    
4. **Documentación:**
    - Dentro de la carpeta `docs`, crea los siguientes archivos de tipo Markdown (.md):
        - `uso_consola.md`: Describe los conceptos aprendidos sobre cómo usar la consola para navegar y crear directorios y archivos. Haz un listado de los principales comandos utilizados en esta unidad.
        - `repositorio_local.md`: Explica cómo crear un repositorio local con comandos de Git.
        - `repositorio_remoto.md` Detalla el proceso para crear un repositorio remoto en GitHub y sincronizarlo con el repositorio local.
5. **Archivo README.md:**
    - En la raíz del proyecto, encontrarás un archivo `README.md`, es este mismo que estás leyendo. Lo vas a editar y vas a incluir al inicio del archivo la siguiente información:
        - Una breve descripción del contenido de tu repositorio. Recuerda que los archivos README.md están ahí para explicarle a las personas que vean tu repositorio, de qué se trata y qué contiene.
        - Explica cuáles son los pasos necesarios para clonar y ejecutar el proyecto.
        - Crea una tabla de contenido con enlaces a los archivos Markdown de la carpeta `docs`.
6. **Uso de Git:**
    - Realiza commits para cada etapa del desarrollo (creación de carpetas, scripts, archivos Markdown, etc.). **Debes realizar mínimo 10 commits.** Los mensajes que utilices deben ser claros, con buena ortografía y con información relevante sobre el cambio que acabas de realizar.
    - Asegúrate de incluir imágenes con pantallazos de los pasos que realices cuando añadas elementos a tu repositorio y de los comandos de Git que utilices y su resultado.
    - Recuerda que los archivos son de Markdown, por lo tanto, debes utilizar los comandos correctos para que los archivos se puedan visualizar de manera correcta.
7. **Entrega:**
    - Sube los cambios en tu proyecto al repositorio remoto en GitHub.
    - Asegúrate de que toda la documentación esté completa y correctamente estructurada.
