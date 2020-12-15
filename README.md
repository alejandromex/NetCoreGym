# Metodo para realizar una app web con ASP.net Core y El entity Framework

## Pasos a seguir

#### Creamos la solucion del proyecto

- dotnet new sln

#### Creamos las clases soluciones

- dotnet new classlib -o Dominio
- dotnet new classlib -o Persistencia
- dotnet new classlib -o Aplicacion

#### Creamos la webapi

- dotnetn new webapi -o WebAPI


#### Iniciamos las Referencias de las clases 


###### Aplicacion -> Dominio && Persistencia

- Entramos a carpeta aplicacion -> dotnet add reference ../Dominio
- Entramos a carpeta aplicacion -> dotnet add reference ../Persistencia

###### WebAPI -> Aplicacion

- Entramos a carpeta WebAPI -> dotnet add reference ../Aplicacion


###### Persistencia -> Dominio

- Entramos a carpeta Persistenca -> dotnet add reference ../Dominio



### Creamos las entidades con EntityFramework (Instalar con paqueteria nuget)
