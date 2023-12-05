# GIT

Algunos comandos

`mkdir nombre-carpeta` -> para crear la carpeta

`cd nombre-carpeta` -> para ir a la carpeta creada

`git init` -> para inciiar el repositorio

Hacemos lo que necesitamos hacer de codigo y luego:

`git add .` -> para agregar los archivos

`git commit -m "aca el mensaje"` -> para el commit


---

Algunos otros comandos útiles:

`git log` -> para ver los logs

1. Para editar git:

Primero:

`git config --global edit` -> para modificar las configuraciones globales de git, para todos los proyectos que utilizo

`git config --local edit` -> para modificar las configuraciones de un proyecto en particular


Segundo:

`:q` -> para salir de VIM


Tercero:

`git config --global core.editor code` y `git config --global edit` para editar con VSC



---

# CLEAN ARQUITECTURE

![image](https://github.com/eugenia1984/clean-arquitecture/assets/72580574/16acb0e8-f739-4584-a727-1f3f59aa9fc3)

- **domain**: las **reglas de negocio**. 

Por ejemplo en un **login** es la `Authentication`, la **interface**.

- **data**: las **implementaciones de los casos de uso**. Tratar resposta de API / tratar erros de API.

Son **clases**. Es la `RemoteAuthentication`, una clase que implementa el protocolo de dominio.  `HttpPostClient` es la **interface**, un protocolo, para el acceso a la API, aca van las reglas.

- **infra**: implementaciones de Frameworks externos. `AxiosHttpClient`, la implementación del protocolo de POST utilizando Axios (la biblioteca externa).



![image](https://github.com/eugenia1984/clean-arquitecture/assets/72580574/5324c6fb-5081-4534-ad06-48069a947dcf)

![image](https://github.com/eugenia1984/clean-arquitecture/assets/72580574/6a4ffb08-b2eb-470a-9645-8ee45db47fd2)

---
