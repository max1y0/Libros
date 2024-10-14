# GitHub
GitHub es un servidor online para alojar proyectos que usan el sistema de control de versiones git.
Es decir, es un servicio que nos permite subir nuestors archivos versionados a un repositorio online, y este no pierde la información de las distintas versiones, ramas, mensajes de cambios, etc.
Además tiene la ventaja extra de que nos permite trabajar colaborativamente a más de un programador en un mismo repositorio.

## Como se usa
Para usar github necesitamos crearnos una cuenta en la página de github. Además tenemos que crear nuestros repositorios remotos desde el sitio web.

Luego configurar desde github nuestro usuario y nuestro email con los siguientes comandos:
```git
git config --global user.name "John Doe"
```
```git
git config --global user.email johndoe@example.com
```

A partir de ahora podemos seguir dos rutas:
### 1. Clonar repositorio
En github, vamos a nuestro repositorio recién creado y copiamos el link que aparece al presionar el boton "Code"

Luego, en nuestra computadora, nos vamos a una carpeta vacía, abrimos una terminal y copiamos el siguiente comando:
```
git clone <link copiado>
```

Esto nos va a crear una carpeta con el nombre de nuestro repositorio en nuestra computadora (Si el repositorio tenía archivos, son descargados). A partir de entonces podemos empezar a trabajar en los archivos como veníamos haciendo con git.

### 2. Agregar un repositorio remoto
En github, vamos a nuestro repositorio recién creado y copiamos el link que aparece al presionar el boton "Code"

En nuestra computadora vamos a la carpeta donde tenemos nuestro proyecto, abrimos una terminal y escribimos:
```
git remote add <link copiado>
```

Esto indica que nuestro repositorio local tiene una copia remota en el link provisto, y vamos a poder subir los cambios al mismo

### Subir y bajar los cambios
Bueno, venimos trabajando en nuestro proyecto, agregamos cambios, hicimos commit de los mismos, y ahora queremos subirlos a github. Para esto necesitamos ejecutar el siguiente comando
```
git push
```
Esto sube los cambios **confirmados con commit** a el repositorio remoto.

De manera análoga, si queremos traer cambios que otro colega hizo y subió al repositorio remoto pero no tenemos en el local, se usa
```
git pull
```

> Entonces, normalmente nuestro flujo de trabajo va a ser similar a este:
> 1. Traer los cambios remotos con ```pull```
> 2. Trabajar en el proyecto e ir agregando cambios con ```add```
> 3. Ir confirmando cambios con ```commit``` y especificando mensajes de versiones
> 4. Al terminar, hacer ```push``` para subir los cambios al repositorio remoto.
