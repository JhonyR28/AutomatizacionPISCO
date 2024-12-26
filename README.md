# AutomatizacionPISCO
## Procesamiento Interactivo de Datos Climáticos PISCO - SENAMHI
El código interactivo procesa datos PISCO de temperatura, precipitación, y caudales, generando archivos Excel adaptados para análisis hidrológicos o integración con el software TETIS. Incluye georreferenciación, opciones de frecuencia, y permite agregar localidades y COMIDs manualmente o desde Excel.
## Se recomienda reiniciar el Kernel para cada petición y trabajar en Google Colab
## Características
* Carga y procesamiento de datos climáticos PISCO:
  * Tmax y Tmin.
  * Precipitación.
  * Evapotranspiración.
  * Caudales (por COMID).
* Personalización:
  * Selección de variables y localidades manual o mediante archivo Excel.
  * Definición de intervalos temporales y frecuencia (diaria, mensual, anual).
* Exportación flexible:
  * Formato Excel estándar para análisis general.
  * Formato estructurado para compatibilidad con TETIS.
* Georreferenciación:
  * Conversión automática de coordenadas y cálculo de elevación.
## Uso
1. Requisitos iniciales:
* Los archivos TMAX.nc, TMIN.nc, Evapotranspiracion.nc, Precipitacion.nc y PISCO_HyD_ARNOVIC_v1.0.nc (archivos renombrados de PISCO de manera DIARIA) deben estar en el directorio de trabajo.
 ### La descarga se tiene a través del siguiente link: https://drive.google.com/drive/folders/1YDtPpIBeltqbiFCZSDexvSmiPRA_4jxi?usp=sharing o también desde https://iridl.ldeo.columbia.edu/SOURCES/.SENAMHI/.HSR/.PISCO/?Set-Language=es seleccionando datos DIARIOS
2. Configuración:
* Ejecuta el código en un entorno Jupyter.
* Carga las dependencias necesarias.
3. Interfaz interactiva:
* Selecciona localidades y variables desde los widgets.
* También se puede añadir un archivo excel con los siguientes formatos.
  ![image](https://github.com/user-attachments/assets/b7885730-a125-427c-8d30-63ba1108d907)
  
* Define el intervalo de tiempo y formato de salida.
4. Generación de resultados:
* Descarga el archivo Excel con los datos procesados.


## Interfaz para TMAX, TMIN, Precipitacion y Evapotranspiracion
![image](https://github.com/user-attachments/assets/a119b1fc-a2d4-4a27-b346-ef619fdb0b85)

![image](https://github.com/user-attachments/assets/395f25cc-511d-42fe-b44f-64be3aa3a835)

## Interfaz para caudales
![image](https://github.com/user-attachments/assets/4d30ecb7-35ef-4678-9ce0-327c01c4f45d)

## Requisitos
* Python 3.7+
* Librerías:
  * folium, geopy, pyproj, requests, geopandas, xlsxwriter, ipywidgets.
Instala las dependencias con:
### pip install folium geopy pyproj requests geopandas xlsxwriter ipywidgets

## Aplicaciones
* Ideal para:

  * Estudios climáticos con datos de PISCO.
  * Modelado hidrológico con integración al software TETIS.
  * Análisis de variabilidad y cambio climático.
  * Este proyecto simplifica el acceso a grandes volúmenes de datos climáticos, generando archivos Excel listos para análisis científico o aplicaciones hidrológicas como TETIS.
