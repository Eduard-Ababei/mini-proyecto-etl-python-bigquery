Mini-Proyecto ETL Python → BigQuery

Este proyecto muestra cómo construir un flujo ETL (Extract → Transform → Load) completo utilizando Python y Google Cloud BigQuery.

El objetivo es practicar la integración entre pandas, las APIs de Google Cloud y un entorno real de ingeniería de datos, gestionando credenciales locales, carga de datos y consultas desde Python.

Objetivos del proyecto

Conectar un entorno Python local con Google Cloud BigQuery mediante credenciales de servicio.

Realizar un flujo ETL completo:

Extract: lectura de datos desde un dataset público (CSV).

Transform: limpieza y agregación con pandas.

Load: carga del resultado en una tabla BigQuery mediante la API oficial.

Validar la carga realizando una consulta SQL desde Python.

Comprender los pasos necesarios para integrar código, nube y datos de forma práctica.

Tecnologías utilizadas
Categoría	Herramienta / Librería
Lenguaje principal	Python 3.x
Data Wrangling	pandas
Cloud Platform	Google Cloud Platform (GCP)
Data Warehouse	BigQuery
API SDK	google-cloud-bigquery
Serialización de datos	pyarrow
Autenticación	application_default_credentials.json
Entorno virtual	venv
Control de versiones	Git y GitHub
Estructura del notebook
Paso	Descripción
1. Dependencias y configuración inicial	Carga de librerías y autenticación con load_credentials_from_file()
2. Lectura del dataset	Descarga del dataset público Iris mediante pandas.read_csv()
3. Transformación	Agregación y cálculo de medias por especie con pandas
4. Carga en BigQuery	Creación de dataset y tabla en BigQuery, y carga del DataFrame con load_table_from_dataframe()
5. Verificación	Ejecución de una consulta SQL desde Python para validar los datos cargados
Resultados

El notebook permite crear un flujo ETL funcional en la nube utilizando BigQuery, demostrando el proceso de integración entre código Python, datasets externos y servicios cloud.
El resultado final es una tabla llamada iris_summary en el dataset demo_dataset dentro del proyecto eloquent-hangar-474417-t1.

Autor: Stefan Eduard Ababei
Proyecto de práctica: Python + Google Cloud BigQuery
