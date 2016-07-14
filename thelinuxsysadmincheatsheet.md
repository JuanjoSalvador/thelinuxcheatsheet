# The Linux Sysadmin Cheatsheet

1. [Comandos auxiliares](#comandos-auxiliares)
2. [Archivos y directorios](#archivos-y-directorios)
3. [Usuarios](#usuarios)
4. [Procesos](#procesos)
5. [Discos](#discos)
6. [Gestión de paquetes](#gestión-de-paquetes)
  1. [APT](#apt)
  2. [YUM](#yum)
  3. [Zypper](#zypper)
  4. [Pacman](#pacman)
  5. [dpkg](#dpkg)
  6. [RPM Package Manager](#rpm-package-manager)
7. [Compresión y descompresión](#compresión-y-descompresión)
  1. [Compresion](#compresión)
  2. [Descompresión](#descompresión)
8. [Filtros](#filtros)
9. [Pipes, redireccionamientos y operadores](#pipes-redireccionamientos-y-operadores)

### Comandos auxiliares

| Comando | Argumento | Descripción                          |
|:-------:|:---------:|:------------------------------------|
| **sudo**| comando   | Ejecuta un comando como superusuario |
| **man** | comando   | Imprime el manual del comando especificado (si existe).
---

### Archivos y directorios

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
| **head** | opción, fichero | Muestra las primeras líneas del fichero indicado. |
| **tail** | opción, fichero | Muestra las últimas líneas del fichero indicado. |
---

### Usuarios

| Comando   | Argumento | Descripción                          |
|:---------:|:---------:|:-------------------------------------|
|**adduser** | | Añade un usuario. |
|**deluser** | | Elimina un usuario. |
|**passwd** | | Permite cambiar la contraseña del usuario actual. |
|**whoami** | | Imprime el nombre del usuario actual. |
|**who** | | Imprime una lista de usuarios con sesión iniciada. |
---

### Procesos

| Comando   | Argumento | Descripción                          |
|:---------:|:---------:|:-------------------------------------|
| **top** | | Muestra en tiempo real los procesos en ejecución. |
|**ps** | opción | Muestra los procesos en ejecución. Ejemplo: ps -e |
|**pidof** | proceso | Muestra el PID del proceso indicado. |
|**kill**| PID | Mata un proceso por PID. |
|**killall** | nombre | Mata un proceso y todos sus hijos, por nombre. |
|**fuser** | puerto/procotolo | Muestra el PID del proceso que está escuchando por el puerto indicado. Ejemplo: 80/tcp |
---

### Discos
| Comando   | Argumento | Descripción                          |
|:---------:|:---------:|:-------------------------------------|
|**mount** |unidad, destino | Monta la unidad especificada. Puede ser una unidad física o lógica. Ejemplo: mount /dev/sda1 /mnt/disk|
|**umount** | unidad | Desmonta la unidad especificada. Ejemplo: umount /dev/sda1|
---

### Gestión de paquetes

#### APT
Distribuciones basadas en Debian/Ubuntu

#### YUM
Distribuciones basadas en RH Linux/Fedora

#### Zypper
Distribuciones basadas en SUSE Linux/OpenSUSE

#### Pacman
Distribuciones basadas en Arch Linux

#### dpkg
Gestor de paquetes DEB

#### RPM Package Manager
Gestor depaquetes RPM

---

### Compresión y descompresión

#### Compresión
| Comando    | Argumento       | Descripción                                                                  |
|:-----------:|:---------------:|:-----------------------------------------------------------------------------|
|**zip**      | destino, origen | Comprime el directorio o fichero indicado en ZIP                             |
|**tar -zcvf**| destino.tar.gz, origen | Empaqueta en formato TAR y comprime el directorio o fichero origen en GZip |
|**tar -cvjf** | destino.tar.bz2, origen | Empaqueta en formato TAR y comprime el directorio o fichero origen en BZ2  |


#### Descompresión
| Comando   | Argumento | Descripción                          |
|:---------:|:---------:|:-------------------------------------|
|**unzip**  |           |                                      |
|**tar**    |           | GZ                                   |
|**tar**    |           | BZ2                                  |
---

### Filtros

Los filtros son comandos especiales que suelen ir concatenados a otro comando.

| Filtro    | Descripción                          |
|:---------:|:-------------------------------------|
|**more** | Filtra el contenido mostrado por pantalla hacia adelante.|
|**less** | Contrario a more.|
|**sort** | Ordena el contenido alfábéticamente.|
|**grep** | Filtra el argumento siguiendo un patrón.|
---

### Pipes, redireccionamientos y operadores

Los pipes, redireccionamientos y operadores son símbolos reservados que nos ayudan a concatenar comandos.

| Operador | Descripción                                                               |
|:--------:|:--------------------------------------------------------------------------|
| `>`  | Redirecciona la salida del comando hacia otro comando o fichero.              |
| `>>` | Funciona como >, pero si se manda a un fichero, no sobreescribe.              |
| `<`  | Redirecciona un fichero como entrada para un comando.                         |
| `&&` | Operador AND. Si el primer comando finaliza con éxito, ejecuta el siguiente.  |
| `||` | Operador OR. Si el primer comando NO finaliza con éxito, ejecuta el siguiente.|
| `|`  | Enviando la salida del primer comando como argumento al segundo.              |
---

**Esta obra se distribuye libremente bajo licencia GNU GPLv3.**
