# **Automatización PISCO**
## **Procesamiento Interactivo de Datos Climáticos PISCO - SENAMHI**

El código interactivo procesa datos PISCO de temperatura, precipitación y caudales, generando archivos Excel adaptados para análisis hidrológicos o integración con el software TETIS. Incluye georreferenciación, opciones de frecuencia, y permite agregar localidades y COMIDs manualmente o desde archivos Excel.

---

## **Recomendación**
Se recomienda **reiniciar el kernel** para cada nueva petición y trabajar en **Google Colab** para mayor compatibilidad.

---

## **Características**
- **Carga y procesamiento de datos climáticos PISCO:**
  - Temperatura máxima (**Tmax**) y mínima (**Tmin**).
  - Precipitación.
  - Evapotranspiración.
  - Caudales (por **COMID**).

- **Personalización:**
  - Selección de variables y localidades manualmente o desde archivos Excel.
  - Definición de intervalos temporales y frecuencia (**diaria**, **mensual** o **anual**).

- **Exportación flexible:**
  - Formato Excel estándar para análisis general.
  - Formato estructurado para compatibilidad con el software **TETIS**.

- **Georreferenciación automática:**
  - Conversión de coordenadas y cálculo de elevación.

---

## **Uso**
### 1. **Requisitos iniciales**
- Los archivos necesarios deben estar en el directorio de trabajo:
  - `TMAX.nc`, `TMIN.nc`, `Evapotranspiracion.nc`, `Precipitacion.nc` y `PISCO_HyD_ARNOVIC_v1.0.nc`.
- Descarga los datos desde:
  - [Google Drive](https://drive.google.com/drive/folders/1YDtPpIBeltqbiFCZSDexvSmiPRA_4jxi?usp=sharing)
  - [SENAMHI - IRIDL](https://iridl.ldeo.columbia.edu/SOURCES/.SENAMHI/.HSR/.PISCO/?Set-Language=es) (seleccionar datos **DIARIOS**).

### 2. **Configuración**
- Ejecuta el código en un entorno de **Google Colab**.
- Carga las dependencias necesarias.

### 3. **Interfaz interactiva**
- Selecciona localidades y variables utilizando los widgets.
- También puedes añadir un archivo Excel, los formatos se encuentran al final.
- Define el intervalo de tiempo y el formato de salida.

### 4. **Generación de resultados**
- Descarga el archivo Excel generado con los datos procesados.

---

## **Interfaz**

### **TMAX, TMIN, Precipitación y Evapotranspiración**
![Interfaz 1](https://github.com/user-attachments/assets/a119b1fc-a2d4-4a27-b346-ef619fdb0b85)

![Interfaz 2](https://github.com/user-attachments/assets/395f25cc-511d-42fe-b44f-64be3aa3a835)

### **Caudales**
![Interfaz Caudales](https://github.com/user-attachments/assets/4d30ecb7-35ef-4678-9ce0-327c01c4f45d)

---

## **Datos de COMIDs**
Obtén los COMIDs para caudales desde:  
[Mapa de COMIDs - HLLauca](https://hllauca.github.io/map_product/Identificar_COMID.html)

---

## **Formato Excel para Tmax, Tmin, Precipitacion y Evapotranspiracion**
![Formato Excel](https://github.com/user-attachments/assets/b7885730-a125-427c-8d30-63ba1108d907)

---

## **Formato Excel para Caudales**
![Formato Excel_2](https://github.com/user-attachments/assets/0c7fe21a-14e4-4e02-8fcc-7f1925b5d6de)

---

## **Requisitos**
- **Python** 3.7+
- Librerías requeridas:
  ```bash
  pip install folium geopy pyproj requests geopandas xlsxwriter ipywidgets
