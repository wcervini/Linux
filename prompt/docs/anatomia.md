### 2. Anatomía del Prompt

El **prompt** en Linux proporciona una interfaz visual para que los usuarios ingresen comandos. A continuación, desglosamos los componentes típicos del prompt por defecto:

#### 1. **Usuario**
El primer componente del prompt muestra el **nombre de usuario** que está actualmente conectado al sistema. Esto ayuda a identificar qué usuario está realizando las operaciones en la terminal.

- **Formato típico:** `usuario@hostname`
- **Ejemplo:** `walter@mi_computadora`
  - `walter` es el nombre del usuario.
  - `mi_computadora` es el nombre del sistema o hostname.

Este formato te permite ver claramente qué usuario está conectado y en qué máquina, lo cual es especialmente útil cuando trabajas en entornos multiusuario o en servidores remotos.

#### 2. **Directorio Actual**
El siguiente componente del prompt muestra el **directorio actual** en el que te encuentras. Este componente te indica tu ubicación dentro del sistema de archivos.

- **Formato típico:** `directorio_actual`
- **Ejemplo:** `~/Documentos`
  - `~` representa el directorio home del usuario actual.
  - `Documentos` es una subcarpeta dentro del directorio home.

Si estás en el directorio home del usuario, el prompt puede mostrar `~` como un atajo para representar esa ubicación. Si te encuentras en otro directorio, el prompt mostrará la ruta completa o relativa desde el directorio home.

#### 3. **Símbolo del Prompt**
Finalmente, el prompt suele terminar con un **símbolo** que indica que el sistema está listo para recibir comandos.

- **Símbolo típico para usuarios normales:** `$`
- **Símbolo para el usuario root:** `#`

- **Ejemplo completo de un prompt:** `walter@mi_computadora:~/Documentos$`
  - Aquí, `walter@mi_computadora` muestra el usuario y el hostname.
  - `~/Documentos` muestra el directorio actual.
  - `$` indica que el usuario es un usuario normal.

Cada uno de estos componentes ayuda a proporcionar contexto y orientación al usuario, permitiendo una navegación y gestión más eficientes del sistema desde la línea de comandos.
