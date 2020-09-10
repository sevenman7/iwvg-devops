## [Máster en Ingeniería Web por la Universidad Politécnica de Madrid (miw-upm)](http://miw.etsisi.upm.es)
## Ingeniería Web: Visión General (IWVG) DevOps
> Este proyecto es un apoyo docente de la asignatura. Cada release liberada corresponde al código utilizado en clase del curso indicado

[![GitHub](https://img.shields.io/github/license/miw-upm/iwvg-devops?color=informational)](https://github.com/miw-upm/iwvg-devops/blob/develop/LICENSE.md)
[![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/miw-upm/iwvg-devops?color=informational)](https://github.com/miw-upm/iwvg-devops/releases)
![GitHub Release Date](https://img.shields.io/github/release-date/miw-upm/iwvg-devops?color=informational)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/miw-upm/iwvg-devops)
![GitHub issues](https://img.shields.io/github/issues/miw-upm/iwvg-devops?color=important)
![GitHub closed issues](https://img.shields.io/github/issues-closed/miw-upm/iwvg-devops?color=informational)

### Estado del código
[![Build Status](https://travis-ci.org/miw-upm/iwvg-devops.svg?branch=develop)](https://travis-ci.org/miw-upm/iwvg-devops)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=es.upm.miw%3Aiwvg-devops&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=es.upm.miw%3Aiwvg-devops)
[![BCH compliance](https://bettercodehub.com/edge/badge/miw-upm/iwvg-devops?branch=develop)](https://bettercodehub.com/results/miw-upm/iwvg-devops)
[![Heroku broken](https://iwvg-devops.herokuapp.com/system/version-badge)](https://iwvg-devops.herokuapp.com/swagger-ui.html)

### Tecnologías necesarias
`Java` `Maven` `GitHub` `Travis-ci` `Sonarcloud` `Better Code Hub` `Slack` `Spring-boot` `Heroku` `OpenAPI`

### :gear: Instalación del proyecto
1. Clonar el repositorio en tu equipo, **mediante consola**:
```sh
> cd <folder path>
> git clone https://github.com/miw-upm/iwvg-devops
```
2. Importar el proyecto mediante **IntelliJ IDEA**
   1. **Import Project**, y seleccionar la carpeta del proyecto.
   1. Marcar **Create Project from external model**, elegir **Maven**.
   1. **Next** … **Finish**.

### :book: Diapositivas
* [Diapositivas de DevOps](docs/miw-iwvg-devops-slides.pdf)   

### :movie_camera: Videos (www.youtube.com/miw-upm)
* Lista de reproducción: **IWVG. Devops Software (Curso 2020-21)**

### :dvd: [Plantilla de la práctica en _docs/template-webflux.zip_](docs/template-webflux.zip)

### :page_with_curl: IWVG. Devops. Enunciado de la práctica
> Todo el software deberá estar en ingles.

#### 1. Crear un proyecto (**0.5 pto**)
Crear un proyecto Maven llamado: **iwvg-devops-nombre-apellido**, versión **1.0.0**. Para ello se aporta **zip** de la plantilla.
> Recordar editar el pom y cambiar el nombre del artefacto (artifactId).   
> Recordar cambiar el nombre de la  carpeta.   
> Importarlo desde IntelliJ.   
> Crear un repositorio en GitHub.   

#### 2. Preparar la gestión mediante Scrum (**0.5 pto**)
> Crear un proyecto de gestión en GitHub y prepararlo para la metodología de Scrum (columnas, etiquetas, hitos...).   

#### 3. Sprint 1. Preparación del ecosistema (**2 ptos**)
Se crearán las siguientes 4 historias (**Issues**) pero se trabajarán en las ramas **develop** & **master**.
* :one: Integración con Slack. Incluir captura de pantalla en la carpeta docs del proyecto
* :two: Integración continua con **Travis-CI**. Incluir **Badge** en README con **link** a la cuenta de Travis-CI.
* :three: Análisis del código con **Sonarcloud**. Incluir **Badge** en README con **link** a la cuenta de Sonar.
* :four: Análisis del código con **Better Code Hub**. Incluir **Badge** en README.
* :five: Desplegar en **Heroku**. Incluir **Badge** en README con **link** a la página de **swagger-ui.html**.
> :one:, :two:... representa el orden temporal de desarrollo de los issues.

#### 4. Release (**0.5 pto**)
> Realizar la primera liberación del código (_**v.1.0.0-release**_)

#### 5. Sprint 2. Preparación del software a desarrollar (**2 ptos**)
Se crearán las siguientes 4 historias (**Issues**).
* Clases :one:**Fraction** & :five:**FractionTest**.
* Clases :two:**User** & :three:**UserTest**.
* Clases :four:**UsersDatabase**.
> :one:, :two:... representa el orden temporal de desarrollo de los issues. Cuando un issue se termine se debe incorporar a la rama **develop**. Las clases Point, User, DecimalCollection, Fraction se podrán copiar de las dadas en clase.

> Realizar la segunda liberación del código (_**v.1.1.0-release**_)

#### 6. Sprint 3. Preparación de cuatro búsquedas a partir de las siguientes, según el valor de las primeros cuatro valores distintos del último commit realizado de la liberación anterior, se creará una historia (**Issues**) por cada búsqueda, con el test correspondiente (**3 ptos**).

* `0` Stream&lt;String> findUserFamilyNameInitialByAnyProperFraction();
* `1` Stream&lt;String> findUserIdByAnyProperFraction();
* `2` Fraction findFractionMultiplicationByUserFamilyName(String familyName);
* `3` Fraction findFirstFractionDivisionByUserId(String id);
* `4` Double findFirstDecimalFractionByUserName(String name);
* `5` Stream&lt;String> findUserIdByAllProperFraction();
* `6` Stream&lt;Double> findDecimalImproperFractionByUserName(String name);
* `7` Fraction findFirstProperFractionByUserId(String id);
* `8` Stream&lt;String> findUserFamilyNameByImproperFraction();
* `9` Fraction findHighestFraction();
* `a` Stream&lt;String> findUserNameByAnyImproperFraction();
* `b` Stream&lt;String> findUserFamilyNameByAllNegativeSignFractionDistinct();
* `c` Stream&lt;Double> findDecimalFractionByUserName(String name);
* `d` Stream&lt;Double> findDecimalFractionByNegativeSignFraction();
* `e` Fraction findFractionAdditionByUserId(String id);
* `f` Fraction findFirstFractionSubtractionByUserName(String name);

> Realizar la tercera liberación del código (_**v.1.2.0-release**_)

#### 7. Bug (**1.5 ptos**)
> Suponer que la búsqueda 3 anterior no es buena y se debe proceder a modificarla. Realizar un cambio y proceder a la cuarta liberación del código (_**v.1.2.1-release**_).

### :white_check_mark: Criterios transversales **con pérdida de puntos por falta de calidad**
* Uso correcto del flujo de trabajo ramificado. **Hasta -3 ptos**. 
* Adecuación de la temporalidad de desarrollo según el enunciado. **Hasta -3 ptos**. 
* Mantenimiento de calidad del código según Travis-CI, Sonar, Better Code Hub. Cobertura >= 80%. **Hasta -2 ptos**. 
* Gestión adecuada, completa y equlibrada (estimación, tiempo real...) durante el desarrollo. **Hasta -2 ptos**. 
* Commits correctos y completos. **Hasta -2 ptos**. 
* Código limpio, bien formateado y ordenado. **Hasta -2 ptos**. 
* Uso del ingles. **Hasta -1 pto**.


### :clap: Entraga de la práctica
Indicar como texto en la subida la **URL de GitHub**
> **NOTA. Acordarse de dar al botón de envío**