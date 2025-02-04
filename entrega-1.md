# Entrega 1
## Tabla de contenido
- [1. Documentación de dominios y sub-dominios](#dominios-y-subdominios)
- [2. Documentación del lenguaje ubicuo](#lenguaje-ubicuo)
- [3. Documentación de contextos acotados Item Valor](#contextos-acotados)

## 1. Dominios y subdominios

- [ContextMapper](src/main/cml/salud_tech.cml)


## 2. Lenguaje Ubicuo

### Dominios y subdominios
[Miro](https://miro.com/app/board/uXjVLkjyAUI=/?share_link_id=883331298013)

- ![AS-IS](lenguaje-ubicuo/Dominios%20y%20subdominios%20AS-IS.jpg)

- ![TO-BE](lenguaje-ubicuo/Dominios%20y%20subdominios%20TO-BE.jpg)

### Event Storming 
[Miro](https://miro.com/app/board/uXjVLlMFlq4=/?share_link_id=606522631777)

#### AS-IS

|                                |             | 
|--------------------------------|-------------|
| Actores                        | Equipo de STA (SRE), Proveedores/Partners, Proveedores/Partners, Equipo de STA (Ingestion y limpieza), Equipo de STA (R&D), Equipo de STA(R&D y Ingestion)   |
| Eventos                        | Ambiente privado creado, Datos Preparados, Datos cargados, Datos Anonimizados, Datos crudos borrados, Datos cargados en el ambiente privado, Verificacion iniciada, Datos Verificados, Datos rechazados, Datos agrupados, Segmentacion de modalidades realizada, data frames generados, token unico de paciente obtenido y ligado  a diagnostico y imagenes, Informacion persistida en base de datos   |
| Comandos                       | crear un ambiente privado, preparar datos, Cargar datos a ambiente privado, Borrar datos, Cargar datos en ambiente privado, Verificar datos y agrupar datos, Rechazar datos, Ejecutar pipeline de modalidades y generacion de data frames, Persistir en base de datos   |
| Modelo de lectura              | Data Frames y datos estructurados, Dicom  |
| Sistemas externos              | Provedor cloud  |
| Definiciones                   | Multi-tenant, Anonimizar, imagenes DICOM, ad-hoc, pipeline, parquet, token unico de paciente  |


#### TO-BE

|                                |             | 
|--------------------------------|-------------|
| Actores                        | Equipo de STA (SRE), Proveedores/Partners, Proveedores/Partners, Equipo de STA (Ingestion y limpieza), Equipo de STA (R&D), Equipo de STA(R&D y Ingestion)   |
| Eventos                        | Pais origen detectado, Ambiente privado creado, Datos Preparados, Datos cifrados, Tarea de empezar anonimizacion ejecutada, Datos cargados, Evento lanzado, Patrones detectados, Datos Anonimizados, Datos crudos borrados, Datos cargados en el ambiente privado, Verificacion iniciada, Datos aprobados, Pipeline detenido, Datos aprobados, Ingenieros notificados, Datos agrupados, Segmentacion de modalidades realizada, data frames generados, token unico de paciente obtenido y ligado  a diagnostico y imagenes, Informacion persistida en base de datos   |
| Comandos                       | Detectar pais origen del cliente, Crear ambiente privado en data center de pais de origen, preparar datos, Ejecutar tarea programada de anonimizar, Detectar patrones de anonimizacion, Anonimizar datos, crear un ambiente privado, preparar datos, Cargar datos a ambiente privado, Borrar datos, Cargar datos en ambiente privado, Verificar datos y agrupar datos, Rechazar datos, Ejecutar pipeline de modalidades y generacion de data frames, Persistir en base de datos   |
| Modelo de lectura              | Data Frames y datos estructurados, Dicom  |
| Sistemas externos              | Provedor cloud, Sistema de cifrado de datos  |
| Definiciones                   | Multi-tenant, Anonimizar, imagenes DICOM, ad-hoc, pipeline, parquet, token unico de paciente  |


- [BigPicture - AS-IS](lenguaje-ubicuo/Event%20Storming%20AS-IS.pdf)

![BigPicture - AS-IS](lenguaje-ubicuo/Event%20Storming%20AS-IS.jpg)

- [BigPicture - TO-BE](lenguaje-ubicuo/Event%20Storming%20TO-BE.pdf)

![BigPicture - TO-BE](lenguaje-ubicuo/Event%20Storming%20TO-BE.jpg)

## 3. Contextos-Acotados 
[Miro](https://miro.com/app/board/uXjVLkjyAUI=/?share_link_id=883331298013)

- ![AS-IS](lenguaje-ubicuo/Contextos%20AS-IS.jpg)

- ![TO-BE](lenguaje-ubicuo/Contextos%20TO-BE.jpg)
