# g/re/p: Why this name?

## Introducción

### Grep recibe su nombre (acrónimo) de las siguientes palabras:
- g → Global
- re → Regular expression (expresión RegEx)
- p → Print: Ya que es una herramienta de la línea de comandos, imprime los resultados

### Opciones de uso:
`grep` (para iniciar el comando)
[opciones de comando, { desc = "Rust - Open Cargo.toml"}]
[patrón d, { desc = "Rust - Join linese filtrado]
[archivo(s) o directorio(s) a filtrar]

### `Flags` u opciones de comando:
- `-i` : "Ignore-case", permite no hacer distinción a la hora de filtrar el documento entre mayúsculas y minúsculas.

- `-w` : "Word", permite pasarle como argumento a `grep` una palabra, es decir, una secuencia sin espacios de caracteres.

- `-c` : "Count", hace que grep devuelva el nº de veces que el patrón se ha repetido. Se puede combinar con `-i`.

- `-m NUM` : "Max count", para de filtrar tras encontrar un número NUM de líneas que coincidan. Se puede combinar con `-v` para que pare de filtrar tras NUM líneas sin coincidencias.

- `-e` : "Extend", permite añadir varios patrones a la búsqueda, y también usar patrones que comienzen por "-".

- `-f` : "File", permite indicarle a `grep` el archivo / archivos sobre los que filtrar el patrón.

- `-v` : "inVert", invierte el patrón, mostrando los resultados que NO coinciden con el patrón.

- `--color` : Permite remarcar los patrones y resultados con colores para distinguirlos mejor

- `-l / -L` : "List matches", `-l` indica solo los archivos que tienen una o más coincidencias con el patrón, mostrando solo la primera, mientras que `-L` indica los que NO coinciden con el patrón.

- `-o` : "Only matching", muestra solo las partes de las líneas del archivo que coinciden con el patrón.

- `-q` : "Quiet", no hace output a `stdout` y devuelve `status 0` si se encuentra coincidencia con el patrón.

- `-h / -H` : "Filename", `-H` imprime el nombre de archivo que contiene cada coincidencia, mientras que `-h` suprime los nombres de archivo (es la opción por defecto cuando solo se da un archivo como input a grep).

- `-r` : "Recursive", lee y filtra recursivamente todos los archivos dentro de un directorio.
