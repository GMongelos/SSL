# Instrucciones para correr el programa

Se realizó la instalación en Windows 10. El IDE utilizado fue VS Code. 


Para instalar el compilador, descargarlo de la siguiente página https://www.msys2.org/

Luego de instalar, abrir la terminal de MSYS2(x32 o x64 bits, dependiendo de la arquitectura del SO) y correr el siguiente comando `pacman -Syu` para actualizar los packages y luego `pacman -S mingw-w64-ucrt-x86_64-gcc` para instalar el compilador gcc

Checkear que se haya instalado el compilador. En una terminal de windows, ejecutar `gcc --version`, lo cual nos deberia devolver lo siguiente:

```
gcc.exe (Rev6, Built by MSYS2 project) 13.2.0
Copyright (C) 2023 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

## Para compilar

Ejecutar el siguiente comando, con una consola cuyo directorio sea el de este TP 0: `gcc -o hello.exe hello.c`. La opción -o es para definir el nombre del ejecutable compilado.

En nuestro directorio se debería haber creado un ejecutable .exe llamado "hello.exe". Ahora para ejecutarlo y verificar su output vamos a  ejecutar el siguiente comando `./hello.exe`, lo cual nos debería devolver:

```
Hello, World!
```

Para concuir el propósito de este TP, versionamos el output del programa en el archivo "output.txt" ejecutando el comando `./hello.exe > output.txt`
