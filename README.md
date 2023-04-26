# Examen programación

## Maestría en Ciencia de Datos

**Evaluación 2023, aspirantes extranjeros**

**Presentado por: Ricardo Ortega Bolaños**

El presente repositorio tiene una carpeta `src` donde se encuentra una imagen, un archivo comprimido y un notebook Jupyter, este ultimo fue construido tanto en VSCode como en Colab (debido a lo recursos computacionales con los que contaba).

El notebook (`notebook_Ricardo.ipynb`) contiene (de manera general) lo siguiente:

1. Se descarga y se lee una [Base de Datos](https://www.gob.mx/salud/documentos/datos-abiertos-152127) con los datos de la evolución de COVID en México.

2. Se genera una figura con 3 gráficas, las cuales son la letalidad semanal de COVID a lo largo de la pandemia para México, el estado de Sonora, y el municipio de Hermosillo (en Sonora). Adicionalmente se guarda dicha figura como `figura.png`.

3. Se genera una tabla (dataframe) con el número de ingresados, el número de decesos y el indice de letalidad, calculado por grupo etáreo. Los rangos de edad elegidos son de 0 a 18 años, de 18 a 30 años, de 30 a 60 años y mayores de 60 años. Adicionalmente se guarda el dataframe como `tabla.csv.zip`.


**Para calcular la letalidad se tuvo en cuenta el siguiente enunciado:**

La letalidad se calcula como el acumulado de pacientes que fueron ingresados respecto a la cantidad de pacientes que al final causaron una lamentable defunción. En este caso los acumulados (para la figura) los estamos tomando por semana y únicamente con la fecha de ingreso al sistema hospitalario. Estos son datos únicamente de pacientes que fueron ingresados a hospitalización. La letalidad nos da una idea de la agresividad del virus, sin que esto refleje numeros en forma global (para eso se utiliza el indicador de mortalidad por cada 100 mil habitantes). Toma en cuenta que la única forma de saber si un paciente causo defunción, es porque tiene una fecha de deceso (afortunadamente la gran mayora no tiene fecha de deceso).
