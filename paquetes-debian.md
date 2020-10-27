# Gestión de paquetes en distribuciones basadas en Debian
## APT en Debian, Ubuntu, Linux Mint, y sus diferentes sabores

1. [Instalación y desinstalación de paquetes](#instalación-y-desinstalación-de-paquetes)
2. [Actualización de paquetes](#actualización-de-paquetes)
3. [Limpieza](#limpieza)

### Instalación y desinstalación de paquetes

| Subcomando | Argumento  | Descripción                          |
|:-----------|:----------:|:-------------------------------------|
| install    | nombre del paquete | Descarga e instala el paquete indicado desde los repositorios |
| remove     | nombre del paquete | Desinstala el paquete, si este se encuentra instalado en el sistema |

### Actualización de paquetes

| Subcomando   | Descripción                          |
|:-------------|:-------------------------------------|
| update       | Actualiza los paquetes disponibles desde los repositorios |
| upgrade      | Actualiza los paquetes instalados en el sistema a la versión más reciente de los repositorios locales |
| dist-upgrade | Realiza una actualización completa, incluyendo versión de la distribución, si hubiese |

### Limpieza

| Subcomando   | Descripción                          |
|:------------ |:-------------------------------------|
| autoremove   | Desinstala los paquetes que ya no son necesarios (generalmente utilizados para distintas dependencias) |
| autoclean    | Borra la caché de paquetes disponibles cuya versión sea anterior al actualmente instalado, tras un `upgrade` |
| clean        | Borra completamente la caché de paquetes disponibles |
