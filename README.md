# Introduction 
 
El proyecto de DB es utilizado para almacenar de forma coherente los script de bases de datos
utilizados en el proyecto.

# Getting Started

Los requerimientos básicos para ejecutar los script de bases de datos se detalla a continuación. 

1.	Instale gradle en su equipo
2.	Instale git en su equipo
3.  En el archivo de `application.yml` se debe configurar los parametros de 
conexión de la base de datos para los ambientes de desarrollo(dev), test(test)
y producción(prod).
4.	Para adicionar un nuevo archivo de script de base de datos se debe adicionar su entrada en el
archivo `formacion-master.yml` (el nombre se puede cambiar y adecuarlo a su proyecto. Se debe cambiar 
también en el archivo de `application.yml` en el apartado de `changeLog` colocar el nuevo nombre 
del archivo). Los archivos de configuración se encuentran en la carpera de `resources`.
Los archivos script de SQL se encuentra en la carpeta `resources\db-script`, aunque la extensión 
no es preponderante si es recomendable mantener la prefijo de `.sql`.

# Build and Test

Para ejecutar los script se pueden ejecutar los siguientes comando desde una 
consola o desde su IDE favorito, según el ambiente. Ejecutar con `gradlew.bat` 
para windows o `./gradlew` para sistemas basados en Unix.

- Ejecución desarrollo: `./gradlew runDev`. 
- Ejecución test: `./gradlew runTest`. 
- Ejecución producción: `./gradlew runProd`. 

Las pruebas se realizaron con la base de datos MySQL versión 8, instalada bajo 
contenedor Docker.

# Contribute
 
 Si existe alguna inconsistencia, bug, sugerencia de mejoras, por favor 
 nos la comparte para evolucionar el proyecto.

- [Luis Bertel](mailto:luisbertel@personalsoft.com.co)
- [Fernando Baños](mailto:febanos@personalsoft.com.co)