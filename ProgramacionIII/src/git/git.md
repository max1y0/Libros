# Git

Git es un software de control de versiones creado por Linus Torvalds, el creador de Linux. Para conocer el uso de la herramienta veamos un ejemplo

## Motivación
Supongamos que tenemos que hacer un trabajo práctico para un espacio curricular.
```
trabajopractico.docx
```
Ese trabajo lo fuimos entregando y fuimos recibiendo correcciones, pero por las dudas fuimos guardando los primeros bocetos por las dudas
```
trabajopractico.docx
trabajopracticoVERSION2.docx
trabajopracticoVERSION3.docx
```
Llega la fecha de entrega, hacemos los últimos cambios y nos queda lo siguiente:

```
trabajopractico.docx
trabajopracticoVERSION2.docx
trabajopracticoVERSION3.docx
trabajopracticoFINAL.docx
```

Luego, se nos pide que ese mismo trabajo lo presentemos en un evento estilo "feria de ciencias", "hackaton", o similares. Tenemos que hacer algunas revisiones al trabajo, pero sin perder el original que presentamos para la materia.
```
trabajopractico.docx
trabajopracticoVERSION2.docx
trabajopracticoVERSION3.docx
trabajopracticoFINAL.docx
trabajopracticoFINALHackaton.docx
```
Y de este mismo trabajo pueden venir las revisiones, correcciones, cambios, que pueden generar de nuevo distintas versiones del trabajo original.

> Git nos permite manejar muchas versiones y ramificaciones del mismo archivo sin generar copias confusas. Nosotros seguimos viendo un solo archivo en la carpeta, y con git podemos movernos entre las distintas versiones y ramas.

## Cómo funciona
Al indicar que vamos a usar git para administrar una carpeta, esta pasa a ser un repositorio git. Todos los archivos dentro de esta carpeta empiezan a tener control de versiones. Para que sea simple de entender, vamos a asumir que tenemos una carpeta llamada ```Proyecto``` y dentro de esta un archivo llamado ```trabajo.py```
```
Proyecto/
└─trabajo.py
```
Por un lado git puede llevar el control de las versiones de cada modificación del archivo trabajo.py. En cierta manera podemos pensarlo grágicamente como sigue:
```
VERSIONES EN GIT

trabajo.py
└─Version 0
└─Version 1
└─Version 2
└─Version 3
    └─Version 3.1
└─Version 4
```
Además, podemos manejar distintas ramas de trabajo según divisiones lógicas que necesitemos en nuestro proyecto:
```
RAMAS EN GIT

trabajo.py
└───────── Rama Principal
     └────── Rama Feria de Ciencias
          └─── Rama Hackaton
```
Cada rama teniendo su historial de versiones en sí mismas.

Cuando gestionamos un archivo con git, cada vez que hacemos cambios son detectados por el software. Estos cambios tienen que o agregarse o descartarse. En el caso de ser agregados, los cambios se guardan en un área llamada "Staging Area". Podemos acumular distintos cambios en nuestro staging area antes de confirmarlos y versionarlos. Una vez estamos conformes con los cambios realizados, necesitamos confirmarlos (en terminología de git, hacer ```commit```). Cuando se confirman los cambios, estos generan una versión en el repositorio de git. Luego se vuelve a empezar, se generan nuevos cambios, se agregan, se confirman, y se genera una nueva versión.

## Workflow
Usar git puede ser tan avanzado como uno quiere y necesita, para el enfoque de esta materia solo vamos a usar el sistema de versionado de archivos y la gestión de repositorios remotos (Ver en [GitHub](./github.md))

Git en particular es un CLI, es decir, es un software que se ejecuta mediante lineas de comando en una terminal. En general, nosotros lo vamos a usar con una extensión mediante Visual Studio Code, pero es necesario conocer los comandos para saber cómo funcionan y cuándo usarlos.

### Comandos

* ``` git init ```: Comando para inicializar un repositorio git en la carpeta en donde estamos situados.

* ```git status```: Comando para visualizar el estado del directorio de trabajo: cambios para agregar, y cambios en staging area para commit.

* ```git add <nombre de archivo>```: Este comando agrega los cambios del archivo especificado al staging area.

* ```git commit -m "mensaje descriptivo"```: Este comando confirma todos los cambios acumulados en el staging area (vacíandola). Es buena práctica escribir un mensaje que describe los cambios realizados en general.


Todos estos comandos se pueden usar desde Visual Studio Code desde la terminal, o desde la extensión de git. Si VSC detecta que estamos en un repositorio git, el comando status no es necesario, y nos muestra los cambios con distintos colores en el editor.
