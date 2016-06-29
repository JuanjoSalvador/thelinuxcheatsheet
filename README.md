# The Linux Cheatsheet v2.0

## Comandos auxiliares

| Comando | Argumento | Descripción                          |
|:-------:|:---------:|:------------------------------------|
| **sudo**| comando   | Ejecuta un comando como superusuario |
| **man** | comando   | Imprime el manual del comando especificado (si existe).
---

## Archivos y directorios

| Comando   | Argumento | Descripción                          |
|:---------:|:---------:|:-------------------------------------|
| **ls**    |opcion, directorio | Lista el directorio indicado, por defecto, el actual. |
| **mkdir** | ruta      | Crea un directorio en la ruta especificada. Si solo se le pasa un nombre, lo crea en la ruta actual. |
| **cd**    | ruta      | Cambia de directorio a la ruta indicada. |
| **pwd**   |           | Imprime la ruta actual. |
| **cp**    | origen, destino | Copia un fichero a otra ruta. Para copiar un directorio completo, hazlo recursivo con cp -r. |
| **mv** | origen, destino | Mueve un directorio o fichero a la ruta indicada. |
| **rm** | fichero o directorio | Elimina el fichero o directorio indicado. Para borrar un directorio que no esté vacío, hazlo recursivo con rm -r.  |
| **cat** | fichero | Imprime por pantalla el contenido del fichero indicado. |
| **find** | ruta, opcion, palabra clave| Busca en la ruta indicada todos los ficheros que contengan la palabra clave. |
| **whereis** | fichero | Similar a find, pero asume que conoces el nombre del fichero. |
| **ln** | origen, destino | Crea un enlace duro o simbólico del fichero o directorio. |
| **chmod** | opciones, destino | Cambia los permisos del directorio o fichero indicados. |
| **chown** | usuario, destino | Cambia el propietario del fichero o directorio indicado. |
---



Juan José Salvador Piedra (@Linuxneitor) – http://juanjosalvador.es/

Esta obra se distribuye libremente bajo licencia GNU GPLv3. Puedes obtener una copia de esta hoja de referencia en PDF aquí.
