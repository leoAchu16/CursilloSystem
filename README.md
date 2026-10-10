# cursillo-system

POM padre del proyecto Cursillo. No contiene código: solo centraliza versiones y declara los módulos.

## Estructura esperada

Clonar todos los repos en la misma carpeta:

    CursilloSystem/
    ├── pom.xml            (este repo)
    ├── cursillo-common/
    ├── cursillo-ms-.../
    └── cursillo-ui/

## Requisitos

- Java 21
- Maven 3.9+
- Variable de entorno SUPABASE_DB_PASSWORD

## Build

    mvn clean install -DskipTests
## Ejecutar microservicios

- En Windows:
  $env:SUPABASE_DB_PASSWORD="Cursillo-12345678"
  mvn spring-boot:run