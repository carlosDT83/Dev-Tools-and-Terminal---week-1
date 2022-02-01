# Preguntas y Respuestas - Semana 1

## 1.-¿Como ver los archivos cambiados dentro de cada commit desde git log?

> El comando **git log** muestra los registros de los commit. Si queremos ver esos registros con salidas especificas, hay que agregar opciones y/o parametros al comando.
---
En las salidas producidas por **git log**, por cada *commit* se muestra el autor, fecha y descripción. Sin embargo no se muestra qué archivos fueron modificados, ni cuáles fueron las modificaciones.
---
___
## 2.-¿Cómo ver el contenido de lo que cambió dentro de cada archivo desde git log?

> Para ver el contenido de lo que cambio, hay que agregar una opcion al comando de git log. A fin de poder visualizar las modificaciones realizadas sobre los archivos, es necesario generar el parche (patch) correspondiente a cada commit. Para ello se debe recurrir a la opción -p.
---

## 3. ¿A qué se refiere HEAD en el contexto de git?
> El concepto de HEAD es muy simple: se refiere al *commit* en el que está tu repositorio posicionado en cada momento. Por regla general HEAD suele coincidir con el último commit de la rama en la que estés, ya que habitualmente estás trabajando en lo último.
___
