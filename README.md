El siguiente proyecto abarca desde la extraccion de datos con tecnicas de web escraping usando drission y selenium hasta la creacion de Dim_tables y Fact_tables para consultas por parte del equipo de analisis.
(Añadi el bundle, dos archivos csv, y el archivo con los codigos postales para hacer el cruce, para que puedas probar el pipeline en databricks, en resources esta el el archivo variables.yml donde puedes colocar el nombre del catalog y los schema que deseas utilizar.)
ruta de el archivo con los codigos postales:
/Volumes/real_state_project_bundle/raw_data/catalogo_maestro/CPdescarga.txt
ruta de los archivos csv:
/Volumes/real_state_project_bundle/raw_data/real_state_csv_landing_volume
En este caso se describe el proceso de etl que se llevo acabo en la plataforma Databricks.
La plataforma que se utilizo para guardar la informacion fue aws, el servicio s3.
Se creo una cuenta de administrador que se agrego a un grupo administradores ya que no es recomendable usar la cuenta root.
Los archivos csv se guardan en un directorio llamado landing del buck real_state_location_s3, en este mismo buck es donde se creo el catalog llamado real_state_project.
En el schema raw_data_real_state se creo un volume donde se conecta con el directorio landing donde llegan los archivos csv.



