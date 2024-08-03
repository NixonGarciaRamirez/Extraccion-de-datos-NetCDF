# NetCDF data extraction / Extraccion de datos NetCDF :world_map: :globe_with_meridians: 


## Description

This project aims to facilitate the use of netCDF data, mainly in meteorological topics.

This project is made up of 5 folders:

* Modules: The modules folder contains the functions that can be used to interact with netCDF data.
* XLSM: This is the folder that contains data in Excel, such as the different coordinates that the program will interact with.
* netCDF: This is the folder where the base netCDF data is saved, that is, the original files that will be used.
* nc_out: This is the folder where the cropped and extracted netCDF data is saved.
* csv_out: This is the folder where the time series extracted from the netCDF files are saved.

### Note: A test netCDF file was left in the netCDF folder

## How to use it ??

This project is a set of functions which are divided into 2 modules:

* The E_S_T module (time series extraction): Here there are 2 functions which allow the extraction of time series from necCDF files for one or more specific locations, among the functions present are:
  - extraction_1: This function is responsible for extracting the information from a specific point
  - multiple_extraction: This function allows the extraction of time series from many specific locations, contained within an excel document (a document with the coordinates of the different municipalities of the department of Antioquia was left as proof)
  - Combiacion_df : This function allows that after you extract the multiple time series, you can join them into a single time series, averaging the extracted value.
  

* The T_I module (Image processing): The functions present within this module allow the visualization of the netCDF information on a map, among the functions present are:
  - global_image: This function allows the visualization of the entire netCDF file on a world map (it should be noted that the select the date you want to display)
  - extraction_region: This function allows you to view the netCDF file in an area delimited by 2 coordinates (a minimum lat and lon and a maximum lat and lon), and also allows you to save the cropped netCDF file, so that it is easier to process.


# Version en español

## Descripción
Este proyecto tiene como finalidad, facilitar el uso de los datos netCDF principalmente en temas metereologicos.

Este proyecto esta compuesto por 5 carpetas:

* Modulos: La carpeta modulos es la que contiene las funciones con las que se puede interactuar con los datos netCDF.
* XLSM: Es la carpeta que contiene datos en excel, como las distintas coordenadas con las que va a interactuar el programa.
* netCDF: Es la carpeta donde se guardan los datos netCDF base, o sea, los archivos originales con los que se va a trabajar.
* nc_out: Es la carpeta donde se guardan los datos netCDF recortados y extraidos.
* csv_out : Es la carpeta donde se guardan ls series de tiempo extraidas de los archivos netCDF.


<span  style="color:red;"> Nota: </span >  Se dejo un archivo netCDF de prueba en la carpeta netCDF


## Como usarlo ??

Este proyecto es unc onjunto de funciones las cuales se dividen en 2 modulos:

* El modulo E_S_T (estraccion de serie de tiempo): Aqui se encuentran 2 funciones las cuales permiten extraer las series de tiempo de los archivos necCDF para una o mas ubicaciones especificas, entre las funciones presentes se encuentra:
  - extraccion_1: Estra funcion se encarga de que se extraiga la informacion de un punto en especifico
  - multiple_extraccion: Esta funcion permite que se extraigan las series de tiempo de muchas ubicaciones especificas, contenidas dentro de un documento excel (se dejo un documento con las coordenadas de los distintos municipios del departamento de antioquia como prueba)
  - Combinacion_df : Esta funcion permite que despues deque tu extraigas las multiples series de tiempo, puedas unirlas en una sola serie de tiiempo, promediando el valor extraido.

* El modulo T_I (Tratamiento de imagenes): La funciones presentes dentro de este mudulo permiten la visualizacion en un mapa de la informacion netCDF, entre las funciones presentes se encuentran:
  - imagen_global: Esta funcion  permite vizualizar la totalidad del archivo netCDF en un mapa mundial (cabe resaltar que se debe seleccionar la fecha que se quiere visualizar)
  - extraccion_region: Esta funcion permite vizualizar el archivo netCDF en un area delimitada por 2 coordenadas (una lat y lon minima y una lat y lon maxima), ademas de que te permite guardar el archivo netCDF recortado, esto para que se mas facil procesarlo.
