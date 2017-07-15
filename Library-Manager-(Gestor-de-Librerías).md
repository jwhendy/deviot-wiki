<p align="center">
    <a href="#c%C3%B3mo-usar">Español</a>
</p>

### How to use

Deviot uses a library manager provided by platformio, you can install or delete a library with a few steps.

##### Install Library
`Deviot Menu > Find/Install Library`

##### Remove Library
`Deviot Menu > Remove Library`

Every time you install or remove a library, the menu list `Import Library` and `Examples` are automatically updated.

### Install Library Manually

To manually install a library go to: `Deviot Menu > Library Options > Open Library Folder`

This directory is intended for the project specific (private) libraries.
Deviot (platformIO) will compile them to static libraries and link to executable file.

The source code of each library should be placed in separate directory, like
"lib/private_lib/[here are source files]".

For example, see how can be organised `Foo` and `Bar` libraries:

<p align="center">
    <img src="https://github.com/gepd/Deviot/blob/master/docs/private_library.png?raw=true">
</p>

Then in `main.c` (or what you are using) you should use:

`#include <Foo.h>`

`#include <Bar.h>`

`rest of H/C/CPP code`

Deviot (PlatformIO) will find your libraries automatically, configure preprocessor's
include paths and build them.

See additional options for PlatformIO library dependency finder `lib_*`:

http://docs.platformio.org/en/latest/userguide/lib/index.html

### Cómo usar

Deviot usa el gestor de librerías de platformio, puedes instalar o liminar librerías con solo algunos pasos.

##### Instalar Librería
`Menu Deviot > Buscar/Instalar Librería`

##### Eliminar Librería
`Menu Deviot > Eliminar Librería`

Cada vez que instalas o eliminas una librería, las listas de los menu `Importar Librería` y `Ejemplos` son actualizadas automáticamente.

### Instalar Librería Manualmente

Para instalar una librería manualmente anda a: `Menu Deviot > Opciones de Librería > Abrir Carpeta con Librerías`

Este directorio está destinado para proyectos con librerías específicas (privadas).
PlatformIO compilará las bibliotecas como estáticas y las enlazará a un archivo ejecutable.

El código fuente de cada biblioteca debe ser colocado en una carpeta por separado, "lib/lib_privada/[aquí tu código fuente]"

Por ejemplo, mira como deben ser organizadas las librerías `Foo` y `bar`:

<p align="center">
    <img src="https://github.com/gepd/Deviot/blob/master/docs/private_library.png?raw=true">
</p>

En tu archivo `main.c` (o el que estés usando) deberías usar

`#include <Foo.h>`

`#include <Bar.h>`

`El resto del código H/C/CPP aquí`

Deviot (platformIO) encontrará las librerías automáticamente, y las compilará cuando incluyas su ruta.

Para ver información adicional y más opciones del gestor de librerías de PlatformIO visita (Inglés):

http://docs.platformio.org/en/latest/userguide/lib/index.html
