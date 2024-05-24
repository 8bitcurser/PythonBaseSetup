# PythonBaseSetup

## Descripcion

Primero que nada necesitan saber usar [git](https://www.freecodecamp.org/espanol/news/guia-para-principiantes-de-git-y-github/) y [github](https://github.com/skills/introduction-to-github) esto les va a permitir colaborar entre ustedes sin pisar sus cambios y saber quien hizo que y cuando.

El nivel de complejidad y control que quieran utilizar par sus repositorios depende de ustedes 

En este repositorio les voy a dar una formula basica para que puedan trabajar e instalar librerias en su entorno de trabajo
sin necesitar instalarlas en el sistema base (sus computadoras) y generar conflictos entre versiones; es decir Juan, Pedro y Maria
todos utilizan la misma version de Python y la misma version de las librerias obteniendo todos los mismos resultados independientemente
de que hayan instalado previamente en sus sitemas.

> Pero yo uso Linux, Juanita usa Mac y Pedro Windows

Si bien este entorno les va a facilitar trabajar con la misma "receta" de entorno y solo genere conflictos para instalar en algunos sistemas
particulares es decir en un Apple Silicon M4 para decir algo, no es un reemplazo a que todo el equipo corra el mismo sistema operativo. 
Lo cual no significa comprar todos una computadora e instalar todos el mismo, sino que me refiero a "Virtualizar" una computadora en otra y asi 
como tienen una "receta" para instalar las mismas librerias y version de python, se puede hacer lo mismo para instalar un mismo sistema 
operativo con las mismas aplicaciones dentro de sus sistemas operativos con los que vienen sus computadoras.

> Como seria eso?

Generalmente lo que se utiliza en muchos entonros de trabajo es [Docker](https://www.docker.com/) aca hay una breve [explicacacion](https://www.redhat.com/es/topics/containers/what-is-docker)

> Que deberiamos saber?

Mi consejo es aprendan a utilizar las terminales, esas pantallitas negras donde en las peliculas ingresan comandos y "hackean el mainframe" tanto en 
OSx(Mac) como en Linux se llama "Terminal" en Windows la pueden encontrar como Powershell y los comandos suelen ser diferentes, aprender a manejarse
dentro de este tipo de interfaces es fundamental para su comprension de las computadoras y sentirse mas comodos manipulandolas. Otra recomendacion 
es que instalen un virtualizador de sistemas operativos como lo es [VirtualBox](https://www.virtualbox.org/) e instalen una version de Linux como lo puede ser [Ubuntu](https://ubuntu.com/) para familiarizarse con entornos Unix, creanme lo van a amar eventualmente y les vas a dar mucho mas control. 


## Contenido

Hasta ahora asumo que han utilizado Pip para instalar librerias de python como lo son tensorflow, matplotlib, Pyllow, etc. El problema de usar pip
es que instala esas dependencias en el sistema y eso podria generar conflictos con otros programas que tengan. Otro escenario podria ser si dos de ustedes instalan diferentes versiones de la misma libreria generando 
resultados incongruentes y/o hasta tener diferentes versiones de Python lo cual podria generar todo tipo de problemas. 
Para resolver esto se suelen usar dos cosas, "Entornos virtuales" y "Package Managers" o Adminsitradores de paquetes estos administradores nos permiten
controlar justamente las dos cosas mencionadas anteriormente que version de python usamos y que versiones de las librerias poseemos, de tal forma que si
Maria y Juanita tienen resultados que no condicen pueden comparar que versiones de las librerias estan usando ademas de comparar como escribieron el 
codigo. 

En este repositorio voy a usar [Poetry](https://python-poetry.org/docs/) el facilita 
contener proyectos de python dentro de una carpeta sin afectar lo que pasa fuera de esta, lo cual es muy genial. Imaginense que en su sistema tienen instalado tensorflow 1.0.0 y quieren probar algo nuevo que salio en tensorflow 1.0.2. Si actualizan la libreria en sus sistema "BOOM" varios proyectos que dependian de 1.0.0 podrian romperse, entonces para probarlo de forma segura abren una carpeta, le permiten a poetry inicializar el proyecto e instalan lo que quieran de forma segura.
