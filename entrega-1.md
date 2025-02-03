# Entrega 1
## Tabla de contenido
- [1. Documentación de dominios y sub-dominios](#dominios-y-subdominios)
- [2. Documentación del lenguaje ubicuo](#lenguaje-ubicuo)
- 

## 1. Dominios y subdominios

- [ContextMapper](src/main/cml/salud_tech.cml)

## 2. Lenguaje Ubicuo

### Dominios y subdominios

- [AS-IS](lenguaje-ubicuo/Dominios%20y%20subdominios%20SaludTech%20AS-IS.pdf)

![AS-IS](lenguaje-ubicuo/Dominios%20y%20subdominios%20SaludTech%20AS-IS.jpg)

- [TO-BE](lenguaje-ubicuo/Dominios%20y%20subdominios%20SaludTech%20TO-BE.pdf)

![TO-BE](lenguaje-ubicuo/Dominios%20y%20subdominios%20SaludTech%20TO-BE.jpg)

### Event Storming

#### AS-IS

|                                |             | 
|--------------------------------|-------------|
| Actores                        | Equipo de STA (SRE), Proveedores/Partners, Proveedores/Partners, Equipo de STA (Ingestion y limpieza), Equipo de STA (R&D), Equipo de STA(R&D y Ingestion)   |
| Eventos                        | Ambiente privado creado, Datos Preparados, Datos cargados, Datos Anonimizados, Datos crudos borrados, Datos cargados en el ambiente privado, Verificacion iniciada, Datos Verificados, Datos rechazados, Datos agrupados, Segmentacion de modalidades realizada, data frames generados, token unico de paciente obtenido y ligado  a diagnostico y imagenes, Informacion persistida en base de datos   |
| Comandos                       | crear un ambiente privado, preparar datos, Cargar datos a ambiente privado, Borrar datos, Cargar datos en ambiente privado, Verificar datos y agrupar datos, Rechazar datos, Ejecutar pipeline de modalidades y generacion de data frames, Persistir en base de datos   |
| Modelo de lectura              | Data Frames y datos estructurados  |
| Sistemas externos              | Provedor cloud  |
| Definiciones                   | Multi-tenant, Anonimizar, imagenes DICOM, ad-hoc, pipeline, parquet, token unico de paciente  |


#### TO-BE

|                                |             | 
|--------------------------------|-------------|
| Actores                        | Equipo de STA (SRE), Proveedores/Partners, Proveedores/Partners, Equipo de STA (Ingestion y limpieza), Equipo de STA (R&D), Equipo de STA(R&D y Ingestion)   |
| Eventos                        |    |
| Comandos                       |    |
| Modelo de lectura              |    |
| Sistemas externos              |    |
| Definiciones                   |    |


- [BigPicture - AS-IS](lenguaje-ubicuo/Event%20Storming%20AS-IS.pdf)

![BigPicture - AS-IS](lenguaje-ubicuo/Event%20Storming%20AS-IS.jpg)

- [BigPicture - TO-BE](lenguaje-ubicuo/Event%20Storming%20TO-BE.pdf)

![BigPicture - TO-BE](lenguaje-ubicuo/Event%20Storming%20TO-BE.jpg)