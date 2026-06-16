# Librerías para Proyecto OpenGL

Este repositorio contiene las dependencias necesarias para compilar y ejecutar el proyecto OpenGL.

## Estructura requerida

La carpeta `Librerias` debe ubicarse directamente en la raíz del disco `C:` para que las rutas configuradas en Visual Studio funcionen correctamente.

Ejemplo:

```text
C:\
├── Librerias
│   ├── assimp
│   ├── glew-2.3.1
│   ├── glfw
│   └── glm
```

## Dependencias incluidas

* Assimp
* GLEW 2.3.1
* GLFW
* GLM

## Configuración de Visual Studio

### Include Directories

```text
C:\Librerias\assimp\include
C:\Librerias\assimp\build\include
C:\Librerias\glew-2.3.1\include
C:\Librerias\glfw\include
C:\Librerias\glm
```

### Library Directories

```text
C:\Librerias\glew-2.3.1\lib\Release\x64
C:\Librerias\glfw\build\src\Release
C:\Librerias\assimp\build\lib\Release
```

### Additional Dependencies

```text
glew32s.lib
glfw3.lib
assimp-vc145-mt.lib
Gdi32.lib
Opengl32.lib
User32.lib
Shell32.lib
```

## Importante

Para ejecutar el proyecto es necesario que el archivo:

```text
assimp-vc145-mt.dll
```

se encuentre junto al ejecutable (`.exe`) o que la ruta:

```text
C:\Librerias\assimp\build\bin\Release
```

esté agregada al PATH del sistema.
