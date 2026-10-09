# Ejercicio 1. Entorno de trabajo: control de versiones y contenedores

## Parte A. Investigación

### ¿Qué es un sistema de control de versiones y qué problema resuelve en un trabajo en equipo?

Un **sistema de control de versiones** (**VCS**, por sus siglas en inglés) es una herramienta que permite registrar y administrar los cambios realizados en los archivos de un proyecto a lo largo del tiempo. Permite saber **qué cambió**, **quién lo cambio**, **cuándo lo hizo** y, en muchos casos, **recuperar una versión anterior**.

En un trabajo en equipo, resuelve principalmente el problema de que **varias personas necesiten modificar los mismos archivos SIN perder el trabajo de los demás**. También facilita trabajar simultáneamente, revisar cambios y regresar a una versión anterior si se comete un error.

**Ejemplo:** Supongamos que estudiantes de la ESCOM desarrollan una página web. Un estudiante modifica el menú, otro trabaja el diseño, y otro agrega funcionalidades. Con un sistema de control de versiones, cada integrante puede registrar sus cambios y posteriormente integrarlos en el proyecto común. Si alguien introduce un error, también es posible consultar o recuperar una versión anterior.

### ¿Cuál es la diferencia entre Git y GitHub?

Aunque están relacionados, **Git y GitHub NO son lo mismo**.

#### Git

**Git** es un sistema de control de versiones distribuido. Es un programa que se instala en la computadora y permite registrar cambios, crear *branches*, ralizar *commits* y fusionar modificaciones, entre otras operaciones.

Git se puede utilizar sin conexión a Internet para administrar un proyecto localmente.

#### GitHub

**GitHub** es una plataforma en línea que permite almacenar repositorios Git y colaborar con otras personas. Ofrece herramientas como *Pull Requests*, revisión de código, seguimiento de problemas (*Issues*) y administración de proyectos.

\
Una forma sencilla de entenderlo es:
**Git** es la herramienta de control de versiones y **GitHub** es una plataforma que permite alojar repositorios Git y colaborar sobre ellos.

### Conceptos fundamentales de Git

#### Repositorio

Un **repositorio** es el espacio donde se almacena un proyecto y su historial de cambios administrado por Git. Puede estar en una computadora local o en una plataforma como GitHub.

**Ejemplo:** Este mismo repositorio, que aunque no es un proyecto, contiene todas las prácticas y listas que se realizan durante el desarrollo del curso.

#### *Commit* (Confirmación)

Un ***commit*** es un registro de un conjunto de cambios realizados en un proyecto. Funciona como una *"fotografía"* del estado del proyecto en un determinado momento.

Normalmente, cada *commit* incluye un mensaje que explíca qué se modificó.

**Ejemplo:** ```Update README.md``` -> mensaje que explica que acción se realizó.

#### *Branch* (Rama)

Una **rama *(branch)*** es una línea independiente de desarrollo dentro de un repositorio. Permite trabajar en una característica o modificación **sin alterar directamente la rama principal**.

**Ejemplo:** Un proyecto tiene una rama ```main``` con la versión estable. Un colaborador puede crear una rama llamada ```login``` para desarrollar el inicio de sesión sin modificar directamente el ```main```.

#### *Merge* (Fusión)

Una **fusión *(merge)*** es la operación mediante la cual se incorporan los cambios de una rama a otra.

**Ejemplo:** El colaborador termina de desarrollar el sistema de inicio de sesión en la rama ```login```. Cuando comprueba que funciona correctamente, sus cambios pueden fusionarse con ```main```.

#### *Merge Conflict* (Conflicto de Fusión)

Un **conflicto de fusión *(merge conflict)*** ocurre cuando Git no puede combinar automáticamente dos conjuntos de cambios porque modifican una misma parte de un archivo de manera incompatible.

**Ejemplo:** Dos integrantes modifican exactamente la misma línea. Cuando Git intenta fusionar ambas modificaciones, no sabe cuál de las dos debe conservar. Para resolverlo, los integrantes tienen que resolver manualmente el conflicto y decidir qué versión utilizar.

#### *Pull Request*

Un ***Pull Request*** es una solicitud para incorporar las cambios realizados en una rama a otra rama, normalmente la rama principal. Es una herramienta muy utilizada en GitHub para que otros integrantes revisen el código antes de incorporarlo.

**Ejemplo:** Un integrante termina una nueva función en la rama ```new-function``` y crea un *Pull Request* para solicitar que sus cambios sean incorporados a ```main```. Otro compañero puede sevisar el código, hacer comentarios y aprobarlos.

#### Archivo ```.gitignore```

El archivo ```.gitignore``` indica a Git qué archivos o carpetas debe **ignorar** y, por lo tanto, no debe incluir normalmente en los *commits*.

Es especialmente útil para evitar subir archivos temporales, configuraciones locales, contraseñas, archivos generados automáticamente o entornos virtuales.

**Ejemplo:**
```
venv/
__pycache__/
.env
*.pyc
```
En este caso, Git ignorará el entorno virtual ```venv```, los archivos de caché de Python y el archivo ```.env```.

#### Archivo ```README```

El archivo ```README``` es un documento que proporciona información de un proyecto. Normalmente explica qué hace el proyecto, cómo instalarlo, cómo utilizarlo y otros aspectos importantes.

Un README suele escribirse en formato *Markdown* (*```README.md```*)

**Ejemplo:**
```
# Ejemplo de README

Este es un ejemplo de cómo se ve el código en *Markdown*.

## Ejecución

python app.py
```
El README permite que una persona que nunca ha visto el proyecto pueda entenderlo y comenzar a usarlo.

### ¿Qué es un contenedor y en qué se diferencia de una máquina virtual?

Un **contenedor** es una unidad de software que incluye una aplicación junto con las dependencias y archivos necesarios para ejecutarla de manera consistente en diferentes entornos. Una tecnología muy utilizada para trabajar con contnedores es **Docker**.

La principal diferencua con una **máquina virtual (VM)** es que una máquina virtual incluye un sistema operativo completo virtualizado, mientras que un contenedor comparte el *kernel* del sistema operativo anfitrión.

#### Tabla de Comparación (Contenedor vs Máquina Virtual)

<table>
  <thead>
    <tr>
        <th style="text-align: center;"><b>Característica</b></th>
        <th style="text-align: center;"><b>Contenedor</b></th>
        <th style="text-align: center;"><b>Máquina Virtual</b></th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td style="text-align: center;"><b>Arranque</b></td>
        <td style="text-align: center;">Muy rápido, normalmente en segundos o menos</td>
        <td style="text-align: center;">Más lento ya que debe iniciar un sistema operativo</td>
    </tr>
    <tr>
        <td style="text-align: center;"><b>Tamaño</b></td>
        <td style="text-align: center;">Generalmente pequeño, porqe no inluye un SO completo</td>
        <td style="text-align: center;">Mayor, porque incluye un sistema operativo completo</td>
    </tr>
    <tr>
        <td style="text-align: center;"><b>Aislamiento</b></td>
        <td style="text-align: center;">Aísla aplicaciones y procesos, pero comparte el *kernel* del anfitrión</td>
        <td style="text-align: center;">Proporciona un aislamiento más fuerte mediante un sistema operativo virtualizado</td>
    </tr>
    <tr>
        <td style="text-align: center;"><b>Recursos</b></td>
        <td style="text-align: center;">Suele consumir menos memoria y CPU</td>
        <td style="text-align: center;">Suele requerir más recursos</td>
    </tr>
    <tr>
        <td style="text-align: center;"><b>Uso común</b></td>
        <td style="text-align: center;">Aplicaciones y servicios</td>
        <td style="text-align: center;">Ejecutar sistemas operativos completos</td>
    </tr>
  </tbody>
</table>

### Conceptos: Imagen, Contenedor, Volumen y Puerto Publicado

#### Imagen

Una **imagen** es una plantilla inmutable que contiene todo lo necesario para crear un contenedor: archivos, dependencias, bibliotecas y configuraciones.

**Ejemplo:** Una imagen basada en ```python:3.12-slim``` puede utilizarse como base para crear un contenedor que ejecute una aplicación Python.

#### Contenedor

Un **contenedor** es una instancia en ejecución de una imagen. Una forma sencilla de verlo: 
  
  Imagen = plantilla
  Contenedor = instancia creada a partir de la plantilla

**Ejemplo:** A partir de una imagen de Python se puede crear un contenedor donde se ejecuta una aplicación web.

#### Volumen

Un **volumen** es un mecanismo utilizado para almacenar datos de manera persistente y separada del ciclo de vida del contenedor.

Esto es importante porque los archivos almacenados únicamente dentro de un contenedor puede desaparecer cuando dicho contenedor es eliminado.

**Ejemplo:** Una aplicación puede guardar los datos de una base de datos en un volumen. Si se elimina y vuelve a crear el contenedor, los datos del volumen pueden conservarse.

#### Puerto Publicado

Un **puerto publicado** pernute hacer accesible desde el exterior un puerto que está siendo utilizado por una aplicación dentro del contenedor.

Por ejemplo: ```8080:80```, significa que el puerto 8080 de la computadora anfitriona se conecta al puerto 80 del contenedor.

Así una aplicación que escuvha en el puerto 80 dentro del contenedor puede ser accedido desde el puerto 8080 del equipo anfitrión.

### ¿Qué es un entorno virtual de Python y por qué no modifica la versión del intérprete?

Un entorno virtual de Python ***(Virtual Environment)*** es un entorno aislado que permite instalar paquetes y dependencias para un proyecto sin afectar las instalaciones de otro proyecto.

Por ejemplo, podemos tener:
```
proyecto-A -> Django 4
proyecto-B -> Django 5
```
aunque ambos proyectos utilicen Python instalado en la misma computadora.

Una forma habitual de crear uno es: ```python -m venv venv```, después se activa el entono y se instalan las dependencias necesarias.

#### ¿Por qué no modifica la versión del intérprete?

Porque un entorno virtual **NO es una instalación diferente de Python ni cambia la versión de Python que ya está instalada en el sistema**. El entorno utiliza un **intérprete de Python** asociado a la versión con la que fue creado.

Por ejemplo, si se crea con: ```python3.12 -m venv venv``` el entorno utilizará *Python 3.12*. Si se crea con: ```python3.11 -m venv venv``` utilizará *Python 3.11*.

Por lo tanto, un entorno virtual permite **aislar dependencias**, pero no sirve para cambiar la versión del intérprete que se está utilizando. Para administrar distintas versiones de Python se pueden utilizar herramientas específicas de gestión de versiones.

### ¿Por qué conviene fijar ```python:3.12-slim``` en lugar de utilizar ```python:latest```?

Cuando se crea un contenedor Docker para una aplicación Python, se puede utilizar una imagen como:```FROM python:3.12-slim``` en lugar de ```FROM python:latest```.

La ventaja prinipal es la **reproducibilidad**.

```python:latest``` no representa necesariamente una versión fija de Python. La etiqueta puede apuntar a una versión más reciente en el futuro. Por ejemplo, una aplicación que hoy se construye con una versión determinada podría terminar utilizando otra versión después que la imagen ```latest``` sea actualizada. Esto puede provocar problemas de compatibilidad.

**Ejemplo:** 

Supongamos que hoy construimos una aplicación utilizando: ```FROM python:latest``` y ```latest``` apunta a Python 3.14. Meses después, la etiqueta cambia y apunta a una versión posterior. Al volver a construir el proyecto podríamos obtener una versión diferente de Python y alguna dependencia podría dejar de funcionar correctamente.

En cambio: ```FROM python:3.12-slim``` indica que queremos utilizar la familia **Python 3.12** y la variante **slim** que está diseñada para ser más pequeña que una imagen estándar.

#### Ventajas de fijar la versión

  - **Mayor reproducibilidad:** Las construcciones del proyecto son más predecibles.
  - **Menos sorpresas:** Una actualización automática de ```latest``` no cambia inesperadamente el entorno.
  - **Mayor facilidad para depurar:** Si aparece un problema, sabemos qué versión de Python estaba utilizando el proyecto.
  - **Mejor compatibilidad:** Podemos probar nuestra aplicación específicamente con Python 3.12.
  - **Mayor control de las actualizaciones:** El equipo decide cuándo actualizar la versión de Python.


## Parte B. Repositorio

### Cree una cuenta en GitHub y un repositorio para esta práctica

**Cuenta de GitHub:** [piriart5](https://github.com/piriart5)

**Repositorio de la Materia:** [TeoriaDeLaComputacion_27-1](https://github.com/piriart5/TeoriaDeLaComputacion_27-1)

### Agregue un archivo ```README.md``` con su nombre completo, boleta, grupo, carrera y un índice de esta práctica

**Archivo ```README.md```:** [README.md](./README.md)

### Agregue un archivo ```.gitignore``` que excluya

**Archivo ```.gitignore:```** [.gitignore](/.gitignore)

### 