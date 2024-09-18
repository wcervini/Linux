### Atajo de Teclado `Ctrl + R`: Búsqueda Inversa en el Historial

El atajo de teclado `Ctrl + R` es una herramienta poderosa para mejorar la productividad en la terminal al permitir la búsqueda rápida de comandos previos en el historial.

#### **¿Qué Hace `Ctrl + R`?**

- **Función:** Inicia una búsqueda inversa en el historial de comandos, permitiéndote encontrar comandos que has usado anteriormente de manera rápida y eficiente.

#### **Cómo Usar `Ctrl + R`**

1. **Inicia la Búsqueda:**
   - Presiona `Ctrl + R` para comenzar una búsqueda inversa. Verás el prompt cambiar a `(reverse-i-search)`.

2. **Introduce el Texto de Búsqueda:**
   - Comienza a escribir una parte del comando que deseas buscar. El terminal mostrará el comando más reciente en el historial que coincida con el texto introducido.

3. **Navega por los Resultados:**
   - Si hay múltiples coincidencias, puedes seguir presionando `Ctrl + R` para desplazarte hacia atrás a través de los resultados coincidentes.

4. **Ejecuta o Edita el Comando:**
   - Una vez que encuentres el comando deseado, presiona `Enter` para ejecutarlo.
   - Si deseas editar el comando antes de ejecutarlo, puedes usar las teclas de flecha para mover el cursor y realizar los cambios necesarios.

5. **Salir de la Búsqueda:**
   - Para salir del modo de búsqueda inversa sin ejecutar un comando, presiona `Ctrl + G`. Esto te llevará de vuelta al prompt de comando sin hacer cambios.

#### **Ejemplos de Uso**

- **Buscar un Comando Específico:**
  Si has ejecutado un comando complejo anteriormente y no recuerdas su nombre completo, presiona `Ctrl + R` y comienza a escribir una parte del comando para encontrarlo rápidamente.

  ```bash
  (reverse-i-search)`git': git status
