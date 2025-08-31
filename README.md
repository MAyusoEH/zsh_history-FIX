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

Este proyecto está licenciado bajo la Licencia Creative Commons Atribución 4.0 Internacional (CC BY 4.0)
.

Puedes usar, modificar y distribuir este código de manera libre, pero en caso de usarlo en entornos comerciales, profesionales o estudios, por favor asegúrate de citar adecuadamente a la autoría original, proporcionando un enlace a este repositorio y mencionando que es tu referencia.

**Créditos:** Este código fue desarrollado por [MAyusoEH](https://github.com/MAyusoEH).
