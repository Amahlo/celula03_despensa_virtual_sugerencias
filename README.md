# Célula 03: Despensa Virtual y Sugerencias

**Institución:** CESDE
**Asignatura:** Metodologías Ágiles para la Programación
**Docente:** Jaime Zapata

## Descripción del Proyecto

El módulo **"Despensa Virtual y Sugerencias"** es una funcionalidad desarrollada para el aplicativo **Sazón**, orientada a facilitar la planificación de comidas. Esta herramienta permite a los usuarios registrar y visualizar de manera sencilla los ingredientes que tienen disponibles en sus hogares, evitando compras innecesarias y el desperdicio de alimentos.

A través de un motor de coincidencias, el sistema cruza en tiempo real el inventario del usuario con el catálogo de recetas. Con esta información, la plataforma sugiere qué cocinar, calcula el porcentaje de coincidencia de cada receta y señala los ingredientes faltantes, contemplando además equivalencias y posibles sustituciones.

## Objetivos y Funcionalidades Principales

- **Gestión de despensa:** registro, consulta y eliminación de ingredientes en la despensa virtual de cada usuario autenticado.
- **Motor de coincidencia:** cálculo dinámico del porcentaje de coincidencia ("match") entre los ingredientes disponibles y los requeridos por cada receta, sin almacenamiento estático de resultados.
- **Sistema de equivalencias:** reconocimiento de distintos nombres, marcas o descripciones como un mismo ingrediente mediante el manejo de sinonimias.
- **Trazabilidad:** registro del historial de búsquedas y consultas realizadas por cada usuario.

## Alcance del Módulo

### Inclusiones

- Modelo entidad-relación y script SQL de la base de datos que soporta el módulo.
- Interfaz desarrollada en React y API construida en Spring Boot para las funcionalidades de la despensa y sugerencias.
- Integración y consumo del módulo común de Usuarios y Autenticación (JWT).

### Exclusiones

| Responsabilidad excluida | A cargo de |
|---|---|
| Creación del catálogo maestro de productos y marcas Nutresa | Célula 1 |
| Creación o edición de recetas y su clasificación temática | Célula 2 |
| Cálculo del aporte nutricional o restricciones alimentarias | Célula 4 |
| Planificación de menús semanales | Célula 5 |
| Funcionalidades de comunidad, valoraciones o comentarios | Célula 6 |
| Sistema de mercadeo, campañas y fidelización | Célula 7 |
| Gestión de la autenticación y roles de usuario | Módulo común (docentes) |

## Arquitectura y Stack Tecnológico

El proyecto está construido bajo una arquitectura de tres capas (presentación, lógica de negocio y datos):

| Capa | Descripción | Tecnologías |
|---|---|---|
| **Presentación (Frontend)** | Construcción de la interfaz y la interacción con el usuario | HTML5, CSS3, JavaScript |
| **Lógica de Negocio (Backend)** | Desarrollo de la lógica del sistema y el motor de coincidencia | Java |
| **Datos** | Almacenamiento de inventarios, recetas y equivalencias | MySQL |

**Herramientas de desarrollo:** Visual Studio Code como entorno de desarrollo integrado, y Git junto con GitHub para el control de versiones y el trabajo colaborativo.

## Equipo de Desarrollo (Célula 03)

- Catalina Lombana Osorio
- Deerly Jharik Hernández Misas
- Verónica Ciro Naranjo
- Maiky Santiago Vergara Chavarría
- Hernán Darío Pérez Higuita

## Aspectos Legales y Académicos

Este informe y desarrollo corresponden a un proyecto formativo de carácter netamente académico. Los derechos morales y la propiedad intelectual sobre el contenido, modelo de datos y desarrollo tecnológico pertenecen exclusivamente a los estudiantes creadores, conforme a la legislación colombiana de derechos de autor. Se otorgan al CESDE los permisos necesarios para la consulta, reproducción y distribución del documento con fines educativos e institucionales, sin fines de explotación comercial.
