# Git-Team_Work
Comandos Git de Trabajo en Equipo
Trabajar en equipo en un proyecto de desarrollo de software requiere una buena comprensión y manejo de Git. Aquí te presento una lista de comandos y conceptos más usados y útiles para trabajar en equipo en una empresa:
Trabajar en equipo en un proyecto de desarrollo de software requiere una buena comprensión y manejo de Git. Aquí te presento una lista de comandos y conceptos más usados y útiles para trabajar en equipo en una empresa:

### Comandos Básicos:

1. **`git clone`**: Clonar un repositorio existente.
   
   git clone <URL_del_repositorio>
   

2. **`git pull`**: Actualizar el repositorio local con los cambios más recientes del repositorio remoto.
   
   git pull
   

3. **`git push`**: Subir los cambios confirmados al repositorio remoto.
   
   git push
   

4. **`git status`**: Ver el estado actual de los cambios en el repositorio.
   
   git status
   

5. **`git add`**: Añadir cambios al área de preparación para el próximo commit.
   
   git add <archivo>
   

6. **`git commit`**: Confirmar los cambios con un mensaje descriptivo.
   
   git commit -m "Mensaje descriptivo"
   

7. **`git branch`**: Listar, crear o eliminar ramas.
   
   git branch
   git branch <nombre_de_la_rama>
   git branch -d <nombre_de_la_rama>
   

8. **`git checkout`**: Cambiar entre ramas o restaurar archivos.
   
   git checkout <nombre_de_la_rama>
   git checkout -- <archivo>
   

### Comandos Avanzados:

9. **`git merge`**: Fusionar una rama con otra.
   
   git merge <nombre_de_la_otra_rama>
   

10. **`git rebase`**: Reaplicar cambios de una rama base sobre otra.
    
    git rebase <rama_base>
    

11. **`git cherry-pick`**: Seleccionar y aplicar un único commit de una rama a otra.
    
    git cherry-pick <ID_del_commit>
    

12. **`git revert`**: Deshacer un commit específico creando un nuevo commit.
    
    git revert <ID_del_commit>
    

### Comandos para la Colaboración:

13. **`git remote`**: Administrar conexiones con repositorios remotos.
    
    git remote -v
    git remote add <nombre> <URL_del_repositorio>
    

14. **`git fetch`**: Descargar cambios del repositorio remoto sin fusionarlos.
    
    git fetch <nombre_del_repositorio_remoto>
    

15. **`git pull --rebase`**: Actualizar el repositorio local con los cambios remotos y aplicarlos mediante rebase.
    
    git pull --rebase
    

16. **`git push --force`**: Forzar la actualización remota con los cambios locales. **Usar con precaución**.
    
    git push --force
    








******* TRABAJAR EN UN PROYECTO (EQUIPO)

Exacto, trabajar directamente en la rama `main` o `master` no es una práctica recomendada cuando se trabaja en un proyecto de equipo. La rama `main` o `master` suele utilizarse para reflejar la versión estable del proyecto y no debería contener cambios no probados o en desarrollo.

Aquí te presento una guía básica sobre cómo trabajar en un proyecto de forma adecuada:

### Flujo de Trabajo con Ramas

1. **Clonar el Repositorio**
  
   git clone <URL_del_repositorio>
  

2. **Crear una Rama para Trabajar en una Función o Tarea**
   Antes de empezar a trabajar en una nueva función o tarea, crea una nueva rama:
  
   git checkout -b nombre_de_la_rama
  

3. **Hacer Cambios y Confirmarlos**
   Realiza tus cambios en la rama que creaste y confirma tus cambios regularmente:
  
   git add .
   git commit -m "Mensaje descriptivo de los cambios"
  

4. **Actualizar tu Rama con los Cambios Recientes**
   Antes de enviar tus cambios, asegúrate de que tu rama está actualizada con los cambios más recientes de la rama `main` o `master`:
  
   git checkout main
   git pull
   git checkout nombre_de_la_rama
   git merge main
  

   O si prefieres usar rebase:
  
   git checkout main
   git pull
   git checkout nombre_de_la_rama
   git rebase main
  

5. **Resolver Conflictos (si es necesario)**
   Si hay conflictos entre tus cambios y los cambios más recientes en la rama `main`, resuélvelos manualmente y luego sigue con el proceso de confirmación.

6. **Enviar Cambios al Repositorio Remoto**
   Una vez que tus cambios estén listos y tu rama esté actualizada con los cambios más recientes, puedes enviar tus cambios al repositorio remoto:
  
   git push origin nombre_de_la_rama
  

7. **Crear una Solicitud de Extracción (Pull Request)**
   En plataformas como GitHub o GitLab, crea una solicitud de extracción para que tu equipo revise tus cambios y los integre en la rama `main` o `master`.

### Buenas Prácticas

- **Mantener Ramas Cortas y Frecuentes**: Es recomendable mantener las ramas cortas y realizar commits frecuentes con mensajes descriptivos.
  
- **Revisar Código**: Antes de enviar una solicitud de extracción, realiza una revisión de código para asegurarte de que tus cambios cumplen con las pautas y estándares del proyecto.

- **Integración Continua**: Configura la integración continua para que tus cambios se prueben automáticamente antes de ser fusionados en la rama principal.

Siguiendo este flujo de trabajo y estas buenas prácticas, podrás colaborar de manera efectiva en un proyecto de equipo sin afectar la rama principal y manteniendo un historial de cambios limpio y organizado.


*****************************************************************************

************************** GIT - MANEJO DE VERSIONES ************************


***** PRIMEROS PASOS CON GIT (Configurando GIT - 1ra Vez)

1- Configurar Email -> git config --global user.email "correoexample@gmail.com"

2- Configurar Nombre -> git config --global user.name "Name Example"




   ************************** COMANDOS EN GIT ******************************

** git log -> Ver todos los comentarios.

** git log --oneline -> Muestra todos los comentarios y sus id's de los commit

** git log --oneline --stat -> Muestra la cantidad de cambios realizados en cada commit.

** git log nombrearchivo -> Ver los comentarios de un archivo especifico.

** git log -all


** git status -> Para saber la rama en la que estamos

** git add . -> Agregar los archivos al repositorio

** git pull -> 

** git clone -> Clona un Repositorio.

	git clone https://github.com/usuario/nombre-repositorio.git


** git fetch -> Se trae los cambios del repositorio remoto al repositorio local

** git merge -> Fusiona los cambios con lo que se tenga en el repositorio local.

** git restore . -> restaurar proyecto a su version anterior. (elimina cambios realizados, volviendo al status anterior)


** git branch nombre-rama -> Crear una NUEVA RAMA
** git checkout nombre-rama -> PARA ENTRAR EN UNA RAMA NUEVA

** git branch -m nombre-rama -> 

** git branch -all -> 

** git remote add origin url-repositorio ->

** git push -> 

******************** ACTUALIZAR un proyecto en GitHub ***********************

1- Asegúrate de estar en la rama que contiene tus cambios. Puedes cambiar de rama usando el comando: 

	git checkout nombre_de_la_rama

2- Añade los archivos modificados o nuevos:

	git add .

3- Realiza un commit:

	git commit -m "Mensaje descriptivo de los cambios"

4- Sube los cambios al repositorio remoto:

	git pull origin main

5- Haz un push a la rama

	git push origin main

******************************************************************************


Este comando se utiliza para copiar un repositorio Git existente a tu máquina local.
Inicializar un repositorio Git: git init

Utilizado para convertir un directorio en tu sistema de archivos en un repositorio Git.
Añadir cambios al área de preparación: git add nombre_del_archivo o git add .

Permite agregar archivos modificados o nuevos al área de preparación para ser incluidos en el próximo commit.
Realizar un commit: git commit -m "Mensaje descriptivo"

Confirma los cambios agregados al área de preparación junto con un mensaje descriptivo que explica los cambios realizados.
Verificar el estado de los archivos: git status

Muestra el estado actual de los archivos en tu repositorio, incluyendo cambios sin seguimiento, cambios en el área de preparación y el estado de la rama.
Ver el historial de commits: git log

Muestra una lista de todos los commits en la rama actual, incluyendo información como el autor, fecha y mensaje del commit.
Crear una nueva rama: git branch nombre_de_la_rama

Crea una nueva rama en tu repositorio, permitiéndote trabajar en características o correcciones de errores sin afectar la rama principal.
Cambiar de rama: git checkout nombre_de_la_rama

Cambia de una rama a otra en tu repositorio.
Actualizar tu repositorio local con cambios remotos: git pull

Descarga los cambios más recientes desde el repositorio remoto y los fusiona automáticamente en tu rama local.
Enviar cambios al repositorio remoto: git push

Sube tus cambios confirmados al repositorio remoto.
Resolver conflictos de fusión: Durante un pull o push, es posible que ocurran conflictos de fusión cuando hay cambios simultáneos en la misma parte del código. Debes saber cómo resolver estos conflictos manualmente.




********************* Subir un proyecto a una nueva rama *********************

1- ** Crear una nueva rama localmente: Este comando crea una nueva rama y automáticamente cambia a ella.

	git checkout -b nombre_de_la_nueva_rama


2- ** Agregar y confirmar tus cambios en la nueva rama:

	git add .
	git commit -m "Mensaje descriptivo"


3- ** Enviar la nueva rama al repositorio remoto: Esto establece la nueva rama en el repositorio remoto.
	
	git push -u origin nombre_de_la_nueva_rama

******************************************************************************





*************************** Combinar proyectos *******************************

1- ** Cambia a la rama destino donde deseas fusionar los cambios:

	git checkout nombre_de_la_rama_destino


2- ** Fusiona la rama que deseas incorporar: Este comando fusionará los cambios de la otra rama en la rama actual.

	git merge nombre_de_la_otra_rama

******************************************************************************



*************************** Rebase (Rebasing) *******************************

1- ** Cambia a la rama que deseas rebasear:

	git checkout nombre_de_la_rama_que_quieres_rebasear

2- ** Rebasa la rama objetivo en la rama actual:

	git rebase nombre_de_la_rama_objetivo


Conflictos de fusión y rebase:
Durante una fusión o un rebase, es posible que surjan conflictos si hay cambios en las mismas partes de los archivos en ambas ramas. Si esto sucede, Git te indicará los archivos en conflicto. Deberás resolver manualmente estos conflictos editando los archivos afectados, marcando las partes conflictivas y luego marcándolas como resueltas.

Después de resolver los conflictos, debes añadir los archivos modificados y luego realizar el commit para completar la fusión o rebase.
******************************************************************************


git checkout -b mi-nueva-rama ->   # Crea una nueva rama y hace checkout a la vez

git worktree remove C:/Users/USER/OneDrive/Escritorio/Vue 


git branch -D mi-nueva-rama   ->   # Borra la rama

Cuando se clona un repositorio: git remote -v == git remote add origin 


*** PARA HACER UN MERGE DE UNA RAMA O DE LAS RAMAS, DEBEMOS ESTAR EN LA RAMA PRINCIPAL (RAMA MASTER), ENTONCES:

1- git checkout master           -> PARA ENTRAR A LA RAMA PRINCIPAL

2- git merge nombre_de_la_rama   -> COMBINA LAS RAMAS


!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! ERROR !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

ESTE ERROR OCURRE CUANDO ALGUIEN HA MODIFICADO LA RAMA PRINCIPAL (MASTER) Y LUEGO A TRATADO DE HACER UN MERGE. GIT ENVIA ESTE ERROR PK NO SABE CUAL ES EL CAMBIO CORRECTO Y NOS DA UNA ADVERTENCIA.


si aparece un error con letras azules, presionamos:

	:wq




        <p>Creando una nueva Rama:</p>
        <pre><code>git branch nombre_de_la_rama
                   # o bien
       git checkout -b nombre_de_la_rama
                # Esto es lo mismo que hacer los dos anteriores pasos juntos
        </code></pre>
        
        <p>Listado de ramas:</p>
        <pre><code>git branch
               # muestra las ramas locales y remotas

       git branch -a #  Solo lista las ramas remotas
       git branch -l # Solo lista las ramas locales
       git branch -r # Solo lista las ramas remotas
        </code></pre>

        <h1>Movernos a otra rama:</h1>
        <p>git checkout nombre_de_la_rama</p>


        <p>Volver a la rama principal (master):</p>
        <pre><code>git checkout master
        </code></pre>

        <p>Mergear una rama en la actual (master)</p>
        <pre><code>git merge nombre_de_la_rama
                # Si hay conflictos, Git te avisara y pedira resolverlos
        </code></pre>

        <p>Si no queremos fusionar pero simplemente queremos tener la rama
           sin perder el historial, podemos usar "rebase" en lugar de "merge".
           El rebase pega todos los cambios de la rama a nuestro trabajo actual.</p>
        <pre><code># En vez de
           git merge mi-nueva-rama

        # Hacer esto
           git fetch origin mi-nueva -rama  # Obtener la ultima version de la rama
           git rebase master mi-nueva-rama    # Pegar mis commits al final del master
        </code></pre>

        <h3>Borrar una rama</h3>
        <p>Puedes borrar una rama si ya se ha integrado en otra. Sin embargo, si
           estás trabajando en ella, primero debes unir tus cambios con algo más
           antiguo. Puedes hacerlo así:</p>
        <pre><code>git checkout master   # Volver a master
           git merge mi-nueva-rama     # Fusiona los cambios a master
           git branch -d mi-nueva-rama  # Borra la rama
        </code></pre>
    </div>




----------------------------------------------------------------------------

			    COLABORAR EN GITHUB

** Clonar un Repositorio: 
		
	git clone url_repositorio


** Cuando clonamos un Repositorio, ya no usamos git remote add origin url_repo, usamos git remote -v, y hacemos push a la rama que queremos enviar los cambios.

	git remote -v
	git push origin main


******************************************************************************
FORMA DE TRABAJAR EN EMPRESAS

** Para traer TODO el codigo de la rama hacia nuestra computadora (local)
Crear Repositorio Local

1- Asegurarnos que estamos en la rama master -> 

		git branch -a

2- Traer todo el codigo de la rama master de forma local
	
		git pull origin main 

	
3- PARA NO TRABAJAR EN LA RAMA MASTER, DEBEMOS CREAR una nueva rama, donde haremos los cambios o modificaciones (XXX NO TRABAJAR EN LA RAMA MASTER XXXX)

		git checkout -b nombre_de_la_rama


4- AL TERMINAR, DEBEMOS ENVIAR EL CODIGO AL REPOSITORIO REMOTO PARA QUE PUEDA SER REVISADO Y APROBADO POR LOS ADMINISTRADORES. 
			XXXXXXXXXXXXX PROHIBIDO HACER MERGE XXXXXXXXXXXXXXXX

COMO CREAMOS UNA NUEVA RAMA E HICIMOS CAMBIOS EN ESTA RAMA, DEBEMOS ENVIAR AL REPOSITORIO REMOTO ESTA NUEVA RAMA.
		
		git push origin nombre_dela_rama


5- CUANDO EL ADMINISTRADOR ACEPTA LOS CAMBIOS Y HACE EL MERGE, ESTE ELIMINA LA RAMA, ENTONCES SUPONGAMOS QUE LA RAMA NUEVA SE ELIMINA, Y AL RATO NOS PIDEN HACER CAMBIOS EN ESA RAMA YA ELIMINADA, LO QUE HACEMOS ES LO SIGUIENTE: 

A) ACCEDEMOS A LA RAMA main Y VOLVEMOS A JALAR TODO EL CODIGO DE LA RAMA.
	
	git checkout main
	git pull origin main 


B) CREAMOS UNA NUEVA RAMA PARA HACER LAS MODIFICACIONES

	git checkout -b nombre_de_la_rama

C) AÑADIMOS LOS NUEVOS CAMBIOS Y AÑADIMOS COMMIT

	git add .
	git commit -m "comentario del nuevo feature"


D) ENVIAR (PUSH) LOS CAMBIOS A LA NUEVA RAMA DE NUEVOS CAMBIOS

	git push nombre_de_la_rama


E) EL ADMINISTRADOR REVISARA LOS CAMBIOS Y LOS APROBARA O NO. SI NO LOS APRUEBA Y PIDE CAMBIOS, PODEMOS EDITAR LA MISMA RAMA, YA QUE NO SE HA HECHO EL MERGE, AGREGAMOS LOS NUEVOS CAMBIOS, O MODIFICAMOS EL CODIGO Y VOLVEMOS HACER PULL A LA MISMA RAMA.

e.1) AGREGAMOS LOS NUEVOS CAMBIOS Y HACEMOS COMMIT 
	
	git add .
	git commit -m "agregado cambio solicitado"


e.2) ENVIAR (PUSH) LOS CAMBIOS A LA MISMA RAMA, YA QUE NO SE HA HECHO MERGE

	git push nombre_de_la_rama


e.3) EL ADMINISTRADOR REVISARA Y APROBARA O NO.



******************************************************************************
	
			Forking (& Contributing)

En el contexto de Git y GitHub, un "fork" se refiere a una copia de un repositorio en GitHub que se realiza bajo la cuenta de otro usuario. La acción de hacer un fork permite a un usuario copiar un repositorio ajeno a su propia cuenta, lo que le permite trabajar en una versión del proyecto sin afectar el original.

Aquí hay algunos puntos clave sobre los forks:

Crear una copia independiente: Cuando haces un fork de un repositorio en GitHub, estás creando una copia independiente del repositorio original. Esta copia está bajo tu control y puedes realizar cambios en ella sin afectar al repositorio original.
