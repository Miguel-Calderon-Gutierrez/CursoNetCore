# Curso de NetCore Vaxi

## Versiones del sdk y runtimes de .Net instaladas en tu pc
``` bash
dotnet --info
```

## Generar un archivo de configuracion con una version especifica (crea un archivo global.json)
``` bash
dotnet new globaljson --sdk-version 6.0.411  --force
```

## Antes de crear un proyecto se crea una solución (se crea con el nombre del directorio)
``` bash
dotnet new sln
```

## Crear un proyecto de tipo consola
``` bash
mkdir LeerData
cd LeerData
dotnet new console
```

## Agregar el proyecto a la solución
``` bash
cd ..
dotnet sln add LeerData/LeerData.csproj
```

## Abrir el proyecto en vscode
``` bash
code .
```

## Extensiones de vscode recomendadas para C# y .Net
### C#                         -> Microsoft

>[!NOTE]  
>configurar en el setting.json de la extención estas lineas:

``` bash
"omnisharp.monoPath": "",
"omnisharp.sdkPath": "C:\\Program Files\\dotnet\\sdk",
"omnisharp.path": "latest"
```

### C# Dev Kit                 -> Microsoft
### C# Extensions              -> JosKreativ
### Material Icon Theme        -> Philipp Kief
### Prettier - Code formatter  -> prettier.io
### .NET Install Tool          -> Microsoft

## Configuración de vscode
>[!IMPORTANT]
> Ir a preferencias, luego consiguraciones(settings) y en C# 
> configuration quitar el check de Omnisharp: Use modern Net 

## Genera la carpeta .vscode para la ejecución del proyecto 
  CTRL + SHIFT + P
``` bash
.Net: Generate Assets for Build and Debug
```

## Correr un proyecto
``` bash
dotnet run --project LeerData/LeerData.csproj
```
