# Respuestas de la parte 6

### (a) ¿En qué se diferencian git restore y git revert?
* **git restore:** Se utiliza para descartar cambios locales que aún no han sido guardados en un commit (Se vuelve a poner el archivo tal y como estaba en el último commit). Modifica los archivos.
* **git revert:** Se utiliza para deshacer un commit que ya ha sido guardado o subido. No borra el commit del historial, pero crea un commit nuevo que agrega los cambios inversos para corregir el código de forma segura en repositorios que se compartan.

### (b) ¿Por qué password.txt sigue siendo un problema aunque ya no aparezca en la última versión?
Sigue siendo un problema de seguridad porque Git guarda el historial de todo el proyecto. Aunque el archivo password.txt ya no aparezca en la carpeta de GitHub, cualquier persona puede entrar en los commits anteriores del historial de Git, abrir el commit donde se cometió el error y ver la contraseña.

### (c) ¿En qué se diferencian git rm y git rm --cached?
* **git rm:** Elimina el archivo por completo tanton del repositorio Git como de mi ordenador.
* **git rm --cached:** Elimina el archivo solo en Git, pero mantiene el archivo físico intacto en mi ordenador para que no pierda mis datos locales.