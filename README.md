oracleCakePhp2.X
================

Cakephp 2.x Oracle DBsource 

Se reescribió la librería de Oracle para cakephp 2.X para que funcione correctamente, esta basada en la 
librería subida por Odin88 que no funcionaba correctamente en versiones posteriores 2.0 y 
además se corrigió para funcionar en php 5.4+

Para configurar el archivo Database : app/Config/database.php
Public $default = array(
  	'datasource' => 'Database/Oracle',
		'driver' => 'oracle',
		'connect' => 'oci_pconnect',
		'persistent' => false,
		'host' => 'ip_address',
		'login' => 'username',
		'password' => 'password',
		'database' => 'ip_address:1521/test',
		'prefix' => '',
		'schema' => 'schema_name'
	);
  
El archivo Oracle.php deben colocarlo en /lib/Cake/Model/Datasource/Database
