# SECCION 3: fundamentos de PBI, Creación de informe iteractivo
> Se trabajará con un archivo excel para el ejercicio practico.

## Fuentes de datos en PBI
- Podemos cargar data a nuestro Power BI con la siguiente ruta **Home >>> Data**
- Al ingresar vamos a ver diferentes opciones para cargar la data.
- Cuando cargamos la data (excel) PBI identifica el tipo de archivo y ademas identifica las tablas dentro del archivo.
- Tambien identifica los tipos de datos que tiene la tabla a analizar
- Luego de cargar la data, PBI crea el modelo de datos, lo cual es una representación de los datos del crudo, pero no trabaja sobre el original.

> **NOTA:** Al hacer transformaciones y modificaciones, PBI no va a modificar los datos del crudo u originales.

- PBI optimiza el volumen de la información y por eso muchas veces el PBI tiene un peso menor al excel.

## Power query editor
> Esta seccion o componente de PBI es donde se realiza la organización de los datos. Permiten: explorar, transformar, limpiar y filtrar

El Editor de Power Query es el motor de transformación y preparación de datos que se utiliza en Excel, Power BI y otros servicios de Microsoft. Su función principal es el proceso ETL (Extraer, Transformar y Cargar), permitiéndote conectar cientos de fuentes de datos y limpiarlos.

### Cuando abres Power Query, entras en un entorno diseñado específicamente para la manipulación de datos:

- **La Cinta de Opciones:** Organizada en pestañas como Inicio, Transformar y Agregar columna, donde encuentras herramientas para dividir columnas, agrupar filas o cambiar tipos de datos.

- **Panel de Configuración de la Consulta:** Es la parte más crítica. Aquí verás la sección de Pasos Aplicados. Cada acción que realizas queda grabada en orden cronológico; puedes volver atrás, borrar o editar cualquier paso anterior.

- **Vista Previa de Datos:** La cuadrícula central que te muestra cómo se ve tu información en tiempo real después de cada transformación.

### Power Query está diseñado para automatizar tareas repetitivas:

Conectividad: Puedes extraer datos desde archivos CSV, carpetas completas, bases de datos SQL, páginas web o incluso archivos PDF.

Anulación de dinamización de columnas (Unpivot): Una de las herramientas más potentes para convertir tablas anchas (con meses en las columnas, por ejemplo) en tablas largas, ideales para el análisis de datos.

Columnas Condicionales: Permite crear nuevas columnas basadas en reglas lógicas (similares al SI de Excel) mediante una interfaz visual sencilla.

Lenguaje M: Aunque todo se hace con botones, por detrás Power Query escribe código en un lenguaje funcional llamado M. Los usuarios avanzados pueden editar este código directamente en el Editor Avanzado.

### El Flujo de Trabajo Automático
La mayor ventaja es la reutilización:

- Conectar: Te vinculas a una fuente de datos.

- Transformar: Realizas la limpieza (quitar nulos, corregir fechas, filtrar filas).

- Cargar: Envías los datos limpios a una hoja de Excel o al Modelo de Datos de Power BI.

- Actualizar: Cuando los datos de origen cambian, solo haces clic en Actualizar. Power Query repite todos los pasos grabados automáticamente y te entrega los datos nuevos ya limpios.

## Que ocurre cuando se modifica el archivo original o el crudo de ruta
Normalmente cuando cambiamos la ruta del archivo de donde viene la data, PBI arroja un error y dice que por favor le de la nueva ruta.

- Lo que se puede hacer es ir a: **Archivo >>> Configuraciones >>> Configuracion de origen de datos**
- Se abre una ventana emergente y le decimos cambiar origen y le indicamos la nueva ruta.

Otra cosa que puede suceder es cuando se agregan nuevos datos o nuevas columnas al archivo original

- En esos casos, en PBI lo que hacemos es refrescar en el panel superior para que actualice desde la data del crudo. Debe ser fuera del power query editor.



