### 3. Personalización del Prompt

Personalizar el prompt en Linux te permite adaptar la línea de comandos a tus necesidades y preferencias. A continuación, exploramos cómo puedes modificar y personalizar el prompt, además de los componentes básicos que puedes ajustar:

#### 1. **Formato del Prompt**
El formato del prompt en Bash se define mediante la variable de entorno `PS1`. Puedes personalizarlo cambiando el valor de esta variable en tu archivo de configuración, como `~/.bashrc` o `~/.bash_profile`.

- **Ejemplo de comando para personalizar el prompt:**
  ```bash
  export PS1="\u@\h:\w\$ "

\u representa el nombre del usuario.  
\h muestra el nombre del host.  
\w muestra el directorio de trabajo actual.  
\$ muestra el símbolo del prompt ($ para   usuarios normales y # para el usuario root).

### Personalización del Prompt: Colores y Estilos

Añadir colores y estilos al prompt en Linux puede hacer que sea más fácil de leer y más estéticamente agradable. A continuación, te mostramos cómo puedes aplicar colores y estilos a tu prompt utilizando secuencias de escape ANSI.

#### 1. **Colores Básicos**

Puedes usar secuencias de escape ANSI para cambiar el color del texto en tu prompt. Aquí te mostramos algunos colores básicos y cómo aplicarlos:

- **Colores de Texto:**
  - **Negro:** `\[\e[30m\]`
  - **Rojo:** `\[\e[31m\]`
  - **Verde:** `\[\e[32m\]`
  - **Amarillo:** `\[\e[33m\]`
  - **Azul:** `\[\e[34m\]`
  - **Magenta:** `\[\e[35m\]`
  - **Cian:** `\[\e[36m\]`
  - **Blanco:** `\[\e[37m\]`

- **Ejemplo de uso:**
  ```bash
  export PS1="\[\e[32m\]\u@\h:\w\[\e[0m\] \$ "

    ```
    
* \[\e[32m\] establece el color verde para el texto.
* \[\e[0m\] restablece el color al valor predeterminado después del texto.

### Estilos de Texto en el Prompt

Los estilos de texto en el prompt de Linux te permiten modificar la apariencia del texto en la terminal. Puedes aplicar estilos como negrita, subrayado y parpadeo utilizando secuencias de escape ANSI. A continuación, se presentan los estilos de texto más comunes y cómo aplicarlos:

#### 1. **Negrita**
La negrita hace que el texto aparezca más grueso y destacado.

- **Código ANSI para Negrita:** `\[\e[1m\]`
- **Ejemplo de uso:**
  ```bash
  export PS1="\[\e[1m\]\u@\h:\w\[\e[0m\] \$ "

### Estilo de Texto: Subrayado

El **subrayado** agrega una línea debajo del texto en el prompt, lo que puede ser útil para resaltar información importante o hacer que el texto sea más visible.

#### **Código ANSI para Subrayado**
- **Código:** `\[\e[4m\]`

#### **Ejemplo de Uso en el Prompt**

Para aplicar el estilo de subrayado a tu prompt, puedes modificar la variable de entorno `PS1` en tu archivo de configuración del shell. Aquí tienes un ejemplo de cómo hacerlo en **Bash**:

- **Comando para establecer el prompt con subrayado:**
  ```bash
  export PS1="\[\e[4m\]\u@\h:\w\[\e[0m\] \$ "

### Estilo de Texto: Parpadeo

El **parpadeo** hace que el texto en el prompt parpadee. Sin embargo, ten en cuenta que no todos los terminales soportan este efecto y, en algunos casos, puede no ser visible o ser molesto para la vista.

#### **Código ANSI para Parpadeo**
- **Código:** `\[\e[5m\]`

#### **Ejemplo de Uso en el Prompt**

Para aplicar el estilo de parpadeo a tu prompt, puedes modificar la variable de entorno `PS1` en tu archivo de configuración del shell. Aquí tienes un ejemplo de cómo hacerlo en **Bash**:

- **Comando para establecer el prompt con parpadeo:**
  ```bash
  export PS1="\[\e[5m\]\u@\h:\w\[\e[0m\] \$ "

### Estilo de Texto: Normal

El **texto normal** restablece el estilo y color del texto al valor predeterminado. Se utiliza para cancelar cualquier estilo o color aplicado anteriormente en el prompt.

#### **Código ANSI para Texto Normal**
- **Código:** `\[\e[0m\]`

#### **Ejemplo de Uso en el Prompt**

Cuando personalizas tu prompt con colores o estilos y deseas volver al texto normal después de aplicar un estilo, debes usar el código ANSI `\[\e[0m\]`. Esto asegura que el texto posterior no mantenga los estilos aplicados anteriormente.

- **Comando para establecer el prompt con texto normal después de aplicar otros estilos:**
  ```bash
  export PS1="\[\e[1;34m\]\u@\h:\w\[\e[0m\] \$ "

### Personalización del Prompt en Zsh

Zsh ofrece una gran flexibilidad para personalizar el prompt. A continuación, se presentan ejemplos de cómo aplicar diferentes estilos y colores al prompt en Zsh.

#### 1. **Formato Básico del Prompt**

Puedes definir el formato básico del prompt en Zsh utilizando la variable `PROMPT`.

- **Ejemplo de Prompt Básico:**
  ```zsh
  export PROMPT="%n@%m:%~%# "

### Variables del Prompt en Zsh

En **Zsh**, la variable utilizada para personalizar el prompt es `PROMPT`. Aquí están algunas de las variables más comunes que puedes usar para configurar tu prompt en **Zsh**:

#### **Variables de Usuario y Host**

- **`%n`**: Nombre del usuario.
  - **Ejemplo:** `%n` muestra `walter` si el usuario es `walter`.
- **`%m`**: Nombre del host hasta el primer punto.
  - **Ejemplo:** `%m` muestra `hostname` si el nombre completo del host es `hostname.local`.
- **`%M`**: Nombre completo del host.
  - **Ejemplo:** `%M` muestra `hostname.local`.

#### **Variables del Directorio**

- **`%~`**: Directorio de trabajo actual, con la ruta relativa desde el directorio home. Muestra `~` si estás en el directorio home.
  - **Ejemplo:** `%~` muestra `~/projects` si el directorio actual es `/home/walter/projects`.
- **`%d`**: Directorio de trabajo actual, con la ruta completa.
  - **Ejemplo:** `%d` muestra `/home/walter/projects`.

#### **Variables de Tiempo y Fecha**

- **`%t`**: Hora en formato `HH:MM:SS`.
  - **Ejemplo:** `%t` muestra `14:30:00`.
- **`%D`**: Fecha en formato `día de la semana` y `mes día`.
  - **Ejemplo:** `%D` muestra `Tue Sep 18`.

#### **Variables del Prompt**

- **`%#`**: Símbolo del prompt (`%` para usuarios normales y `#` para el usuario root).
  - **Ejemplo:** `%#` muestra `$` para un usuario normal y `#` para el usuario root.
- **`%d`**: Fecha en formato `día de la semana` y `mes día`.
  - **Ejemplo:** `%d` muestra `Tue Sep 18`.

#### **Ejemplos de Personalización del Prompt en Zsh**

- **Ejemplo de Prompt Básico:**
  ```zsh
  export PROMPT="%n@%m:%~%# "

### Colores en el Prompt de Zsh

En **Zsh**, puedes utilizar códigos de color ANSI para personalizar el color del texto en el prompt. Los códigos de color permiten cambiar el color del texto y del fondo para mejorar la visibilidad y la estética de tu prompt.

#### **Colores de Texto**

Puedes usar los siguientes códigos de color para cambiar el color del texto:

- **`%F{color}`**: Cambia el color del texto.
  - **`black`**: Negro
  - **`red`**: Rojo
  - **`green`**: Verde
  - **`yellow`**: Amarillo
  - **`blue`**: Azul
  - **`magenta`**: Magenta
  - **`cyan`**: Cian
  - **`white`**: Blanco

- **Ejemplo de Prompt con Texto en Color:**
  ```zsh
  export PROMPT="%F{blue}%n@%m%f:%F{green}%~%f%# "
