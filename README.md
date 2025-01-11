# LiteraLura - Sistema de Gestión de Libros

## Descripción
LiteraLura es una aplicación Java que integra la API de Gutendex para gestionar una biblioteca digital. El sistema permite buscar, almacenar y analizar información sobre libros y autores, ofreciendo una interfaz por consola para interactuar con diversas funcionalidades.

## Capturas de Pantalla

### Menú Principal
![Menú Principal de LiteraLura](https://firebasestorage.googleapis.com/v0/b/chateapp-latino.appspot.com/o/Alura%2FLiteralura%20opciones%20inicial.jpg?alt=media&token=f7d69cc2-fcfd-42f9-b81e-b2b1deaf9cdc)
*Interfaz principal del sistema mostrando todas las opciones disponibles*

### Ejemplo de Búsqueda
![Resultado de Búsqueda](https://firebasestorage.googleapis.com/v0/b/chateapp-latino.appspot.com/o/Alura%2Feligiendo%20opcion%20literalura.jpg?alt=media&token=4e122ef1-040f-4585-9d1a-6fb81fffa6db)
*Ejemplo de resultado al buscar la opcion 8 del top 10*

## Características Principales

### Gestión de Libros
- Búsqueda de libros por título
- Listado de libros registrados
- Filtrado de libros por idioma
- Ranking de los 10 libros más descargados

### Gestión de Autores
- Búsqueda de autores por nombre
- Listado completo de autores registrados
- Filtrado de autores por año de nacimiento
- Filtrado de autores por año de fallecimiento
- Búsqueda de autores vivos en un año específico

### Estadísticas
- Cantidad media de descargas
- Cantidad máxima de descargas
- Cantidad mínima de descargas
- Total de registros evaluados

## Tecnologías Utilizadas
- Java
- Spring Boot
- PostgreSQL
- Maven
- API Gutendex

## Requisitos Previos
- Java 11 o superior
- PostgreSQL
- Maven
- IDE (recomendado: IntelliJ IDEA)

## Configuración del Entorno

### Base de Datos
1. Crear una base de datos en PostgreSQL llamada `literalura`
2. Configurar las variables de entorno:
   - `DB_HOST`: Host de la base de datos
   - `DB_USER`: Usuario de PostgreSQL
   - `DB_PASSWORD`: Contraseña de PostgreSQL

### Variables de Entorno
```properties
spring.application.name=desafioapilibros
spring.datasource.url=jdbc:postgresql://${DB_HOST}/literalura
spring.datasource.username=${DB_USER}
spring.datasource.password=${DB_PASSWORD}
spring.datasource.driver-class-name=org.postgresql.Driver
spring.jpa.hibernate.ddl-auto=update
```

## Instalación y Ejecución

1. Clonar el repositorio:
```bash
git clone [https://github.com/DavidGMc/LiteraLura.git]
```

2. Navegar al directorio del proyecto:
```bash
cd literalura
```

3. Compilar el proyecto:
```bash
mvn clean install
```

4. Ejecutar la aplicación:
```bash
mvn spring-boot:run
```

## Uso
Al iniciar la aplicación, se mostrará un menú con las siguientes opciones:

1. Buscar libro por título
2. Buscar autor por nombre
3. Listar libros registrados
4. Listar autores registrados
5. Listar autores vivos en un determinado año
6. Listar libros por idioma
7. Estadísticas generales
8. Top 10 libros más descargados
9. Listar autores nacidos en algún año
10. Listar autores fallecidos en algún año

Como se muestra en la captura de pantalla del menú principal, la interfaz es intuitiva y fácil de usar. Los resultados se presentan de manera clara y organizada, tal como se puede ver en la imagen de ejemplo de búsqueda.

## Contribución
Si deseas contribuir al proyecto, por favor:
1. Haz un Fork del repositorio
2. Crea una nueva rama para tus cambios
3. Envía un Pull Request con tus mejoras

## Autor
[CD Gonzalez----Androidavid.com]

## Licencia
Este proyecto está bajo la Licencia ----[TIPO_DE_LICENCIA]
