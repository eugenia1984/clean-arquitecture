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

## Clean ARquitecture

Login...

```
...renderizar view
...validar senha
...tratar resposta de APi
...tratar Erros da API
...Controlar Estado
...Comunicar com API
...Regras de Negócio
...Navegação
...Grava dados no Cache
...Validar Email
```



Main
```
Login Factory
Index
DI
```

Validation
```
RequiredFieldValidation    EmailFieldValidation
      |                       |
      v                       v
```

Precentation
```
   |
   v
Validation<---Login   
                |
                v
```

Domain
```
  |
  v
Authentication
  ^
  |  
```

Data
```
  ^
  |
RemoteAuthentication<--HttpPostClient
                            ^
                            |  
```

Infra
```
   ^
   |
AxiosHttpsClient
   |
   v
```

```
  |
  v
Axios
```
