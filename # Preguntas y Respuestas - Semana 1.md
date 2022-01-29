# Preguntas y Respuestas - Semana 1

## 1.-¿Como ver los archivos cambiados dentro de cada confirmación del registro de git?

> Se puede ver desde la pagina web de git o acceder desde la terminal.
---
1. Desde la página web:
    - Se debe ir a la página principal del repositorio que se desea ver en github.com . 
    - Debajo del nombre del repositorio, se debe hacer clic en la pestaña **Insights**.
    - En la barra lateral izquierda, se debe hacer clic en la sección **Commits**.
2. Desde la terminal:
    - Si corresponde, de debe clonar primero el repositorio que se desea ver. En caso contrario, se debe ir desde la terminal, hasta la ubicación del repositorio.
    - Se debe ejecutar el comando **git log**.
___

## 2.-¿Cómo ve el contenido de lo que cambió dentro de cada archivo del registro de git?

> Se puede ver desde la pagina web de git o acceder desde la terminal.
---
1. Desde la página web:
    - Se debe ir a la página principal del repositorio que se desea ver en github.com . 
    - Debajo del nombre del repositorio, se debe hacer clic en la pestaña **Insights**.
    - En la barra lateral izquierda, se debe hacer clic en la sección **Code frecuency**.
    - Se puede hacer una comparación mas detalladas entre commits, en la sección code.
2. Desde la terminal:
    - Si corresponde, de debe clonar primero el repositorio que se desea ver. En caso contrario, se debe ir desde la terminal, hasta la ubicación del repositorio.
    - Se debe ejecutar el comando **git status**.
    - Para hacer una comparacion más detalladas de commits, se pueden usar una serie de comandos:
        - git diff HEAD^ HEAD: En este comando HEAD^ representa el penúltimo commit y HEAD representa al último commit.
        - git diff HEAD^.. --name-status: Si en vez los cambios realizados, queremos ver los archivos que se han visto modificados en el último commit, podemos ver el listado de esos archivos.
        - git diff HEAD^.. -- ./archivo1.txt: Si esos cambios han implicado la modificación de muchos archivos, y queremos únicamente centrarnos en los cambios realizados en uno especifico.
        - git diff HEAD^.. --stat: Si queremos ver un listado rápido de los archivos modificados junto con las modificaciones que se han realizado en ellos.
        - git diff HEAD~3 (nro. especifico): Si queremos contrarnos en un numero especifico de commits.
___
## 3. ¿A qué se refiere HEAD en el contexto de git?
> El concepto de HEAD es muy simple: se refiere al *commit* en el que está tu repositorio posicionado en cada momento. Por regla general HEAD suele coincidir con el último commit de la rama en la que estés, ya que habitualmente estás trabajando en lo último.
___
