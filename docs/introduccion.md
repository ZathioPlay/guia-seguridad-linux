# Introducción y Arquitectura de Git

**Git** es un sistema de control de versiones distribuido (DVCS) creado por Linus Torvalds que permite registrar cada cambio realizado sobre los archivos de un proyecto a lo largo del tiempo, facilitando el trabajo simultáneo de varios desarrolladores sin sobrescribir su código.

## Los tres estados principales de Git

Para dominar Git es fundamental comprender las tres áreas por las que pasan los archivos dentro de tu equipo local:

1. **Directorio de trabajo (*Working Directory*):** Es la carpeta visible donde editas, creas o borras tus archivos.
2. **Área de preparación (*Staging Area / Index*):** Es una zona intermedia donde seleccionas qué cambios concretos formarán parte de la siguiente instantánea.
3. **Repositorio local (`.git`):** Es la base de datos oculta donde Git almacena de forma permanente el historial completo de confirmaciones (*commits*).

## Esquema del flujo de trabajo

En el siguiente diagrama se ilustra el recorrido de los cambios desde el directorio local hasta el repositorio remoto en la nube:

![Arquitectura y flujo de trabajo de Git](img/arquitectura.png)

??? note "Diferencia clave entre Git y GitHub"
    * **Git** es la herramienta local que se instala en tu ordenador y gestiona el historial de versiones en la carpeta oculta `.git`.
    * **GitHub** es la plataforma en la nube que aloja una copia remota de ese repositorio para compartirlo con compañeros, revisar cambios y publicarlo en Internet.

Para profundizar en la referencia técnica oficial, consulta el [libro oficial Pro Git](https://git-scm.com/book/es/v2).
