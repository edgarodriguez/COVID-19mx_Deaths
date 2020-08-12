# COVID-19mx_Deaths
Efecto COVID-19 en el total de defunciones en México.

This visualization is an Exploratory Data Analysis of the effect of COVID-19 and its impact in the mortality rate in Mexico.
In addition, it analyses other death causes that could be related.
## Data source:

1.SEED http://www.dgis.salud.gob.mx/contenidos/basesdedatos/cubos_seed.html
2. Dato oficial COVID19  https://coronavirus.gob.mx/datos/#DownZCSV (8-ago-2020).
3. Proyecciones de Población 1990-2030 CONAPO  http://www.dgis.salud.gob.mx/contenidos/basesdedatos/bdc_poblacion_gobmx.html

## Data cleaning Script:
The data cleaning proccess has several steps and files. (IF YOU COULD HELP WITH CONNECTIVITY WITH MSOLAP WOULD BE GREAT).
1. FILE: Convert MSOLAP to Tabular.twb
  I use native connector of Tableau (Microsoft Analysis Services) to read cubes from source 1. Pass and username could be found when you inspect URL from source 1.
2. FILE: Defunciones_tabular_SEED.xlsx
  Each sheet has a it similar in FILE 1. When you update MSOLAP you only need copy paste each worksheet into Excel and save.
3. FILE: Defunciones_y_poblacion_Mex.tfl
  Tableau Prep file read all data source and arrange, merge, homologate categories and generate final files that Tableau will read.
  For source 2. Only download zip file, extract csv, and delete date from the name.
  For source 3. Copy Dinamic View from cube into a new Excel file and name it properly.
  
## Data visualization

1. FILE: DefuncionesCOVID19-Mexico.twb
  This file include all worksheets and dashboard used in the Visualization.
  
  
 
