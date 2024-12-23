# AutomatizacionPISCO
## Procesamiento Interactivo de Datos Climáticos PISCO
Este proyecto permite manejar y procesar datos climáticos del sistema PISCO. Genera archivos Excel con las variables seleccionadas (Tmax, Tmin, precipitación y evapotranspiración) en formatos adaptados para uso general o para el software hidrológico TETIS.

## Características
* Carga y procesamiento de datos climáticos PISCO:
  * Tmax y Tmin.
  * Precipitación.
  * Evapotranspiración.
* Widgets interactivos:
  * Selección de localidades y variables.
  * Definición de intervalos temporales.
  * Generación de resultados en formatos específicos.
* Exportación flexible:
  * Formato Excel estándar para análisis general.
  * Formato estructurado para compatibilidad con TETIS.
* Georreferenciación:
  * Conversión automática de coordenadas y cálculo de elevación.
## Uso
1. Requisitos iniciales:
* Los archivos TMAX.nc, TMIN.nc, Evapotranspiracion.nc y Precipitacion.nc (archivos renombrados de PISCO de manera DIARIA) deben estar en el directorio de trabajo.
* La descarga se tiene a través del siguiente link:
2. Configuración:
* Ejecuta el código en un entorno Jupyter.
* Carga las dependencias necesarias.
3. Interfaz interactiva:
* Selecciona localidades y variables desde los widgets.
  ![image](https://github.com/user-attachments/assets/b7885730-a125-427c-8d30-63ba1108d907)

* Define el intervalo de tiempo y formato de salida.
4. Generación de resultados:
* Descarga el archivo Excel con los datos procesados.


## Interfaz
![image](https://github.com/user-attachments/assets/a119b1fc-a2d4-4a27-b346-ef619fdb0b85)

## Requisitos
* Python 3.7+
* Librerías:
  * folium, geopy, pyproj, requests, geopandas, xlsxwriter, ipywidgets.
Instala las dependencias con:

- pip install folium geopy pyproj requests geopandas xlsxwriter ipywidgets

## Aplicaciones
* Ideal para:

  * Estudios climáticos con datos de PISCO.
  * Modelado hidrológico con integración al software TETIS.
  * Análisis de variabilidad y cambio climático.
  * Este proyecto simplifica el acceso a grandes volúmenes de datos climáticos, generando archivos Excel listos para análisis científico o aplicaciones hidrológicas como TETIS.
