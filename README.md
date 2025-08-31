## Vista Previa del error:
![Captura de pantalla del proyecto](https://github.com/MAyusoEH/zsh_history-FIX/blob/main/pic_zsherror.png)


## ¿Qué hace este FIX?:
Mueve el historial corrupto a un archivo de respaldo:
``mv ~/.zsh_history ~/.zsh_history_bad``

Extrae solo las cadenas de texto legibles del archivo corrupto:
``strings ~/.zsh_history_bad > ~/.zsh_history``

Fuerza la recarga del nuevo historial en la sesión actual de Zsh:
``fc -R ~/.zsh_history``

Elimina el archivo de respaldo con el historial corrupto:
``rm ~/.zsh_history_bad``


## Cómo usar:

1- Descargar el repositorio al equipo local con la siguiente línea:

``git clone https://github.com/MAyusoEH/zsh_history-FIX.git`` 

2- Dar permisos de ejecución al archivo "fix.sh":

``chmod +x fix.sh``

3- Ejecutar el archivo "fix.sh":

``./fix.sh``


## Licencia:

Este proyecto no está licenciado, el código usado es ampliamente conocido y de dominio público.

**Créditos:** Este archivo fue montado por [MAyusoEH](https://github.com/MAyusoEH).
