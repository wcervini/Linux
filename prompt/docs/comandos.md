### Comandos Útiles para el Prompt

Estos comandos te ayudarán a trabajar con el prompt y gestionar tu entorno de terminal. A continuación se presentan comandos comunes para **Bash**, **Zsh**, y **Fish**.

#### **1. Ver el Directorio de Trabajo Actual**

- **`pwd`**: Muestra el directorio de trabajo actual.
  - **Uso:**
    ```bash
    pwd
    ```
  - **Ejemplo de Salida:**
    ```bash
    /home/walter/projects
    ```

#### **2. Cambiar el Directorio Actual**

- **`cd`**: Cambia el directorio de trabajo actual.
  - **Uso:**
    ```bash
    cd /ruta/del/directorio
    ```
  - **Ejemplos:**
    - **Ir al directorio home del usuario:**
      ```bash
      cd ~
      ```
    - **Subir un nivel en el árbol de directorios:**
      ```bash
      cd ..
      ```

#### **3. Crear Alias para Comandos Comunes**

Los alias permiten crear comandos personalizados para simplificar tareas comunes. Puedes definir alias en el archivo de configuración de tu shell.

- **Bash:**
  - **Definir un alias temporal:**
    ```bash
    alias ll='ls -la'
    ```
  - **Definir un alias permanente:**
    Añade el alias a `~/.bashrc`:
    ```bash
    alias ll='ls -la'
    ```
    Luego recarga el archivo:
    ```bash
    source ~/.bashrc
    ```

- **Zsh:**
  - **Definir un alias temporal:**
    ```zsh
    alias ll='ls -la'
    ```
  - **Definir un alias permanente:**
    Añade el alias a `~/.zshrc`:
    ```zsh
    alias ll='ls -la'
    ```
    Luego recarga el archivo:
    ```zsh
    source ~/.zshrc
    ```

- **Fish:**
  - **Definir un alias temporal:**
    ```fish
    alias ll='ls -la'
    ```
  - **Definir un alias permanente:**
    Usa el comando `funcsave` para guardar el alias en `~/.config/fish/functions`:
    ```fish
    function ll
        ls -la
    end
    funcsave ll
    ```

#### **4. Listar Alias Definidos**

Para ver todos los alias definidos en tu sesión actual:

- **Bash y Zsh:**
  ```bash
  alias
