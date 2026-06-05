El siguiente proyecto abarca desde la extraccion de datos con tecnicas de web escraping usando drission y selenium hasta la creacion de Dim_tables y Fact_tables, ademas de data para crear modelos de machine learning.
En este caso se describe el proceso de etl que se llevo acabo en la plataforma Databricks.
La plataforma que se utilizo para guardar la informacion fue aws, el servicio s3.
Se creo una cuenta de administrador que se agrego a un grupo administradores ya que no es recomendable usar la cuenta root.
Los archivos csv se guardan en un directorio llamado landing del buck real_state_location_s3, en este mismo buck es donde se creo el catalog llamado real_state_project.
En el schema raw_data_real_state se creo un volume donde se conecta con el directorio landing donde llegan los archivos csv.
Se creo una tabla con sql que contiene el nombre de los archivos para despues usarse en la ingestion.
