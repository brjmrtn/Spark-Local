		INSTALAR SPARK EN LOCAL:

	Descargamos Spark de la página https://spark.apache.org/downloads.html. Una vez descargado lo descomprimimos.

	Buscamos el archivo log4j.properties.template y ponemos en log4j.rootCategory=ERROR en vez de INFO.

	Instalamos Anaconda de https://www.anaconda.org

	Descargamos winutils.exe(Binario de Hadoop para Windows) del repositorio https://github.com/steveloughran/winutils/. Buscamos la version de Hadoop con que hemos instalado Spark. Winutils.exe se encuentra en la carpeta bin.


	Nos descargamos e instalamos JAVA si no lo tenemos (Version 7.x o superior) https://www.oracle.com/java/technologies/download/

	Añadimos winutils.exe a una carpeta de winutils\bin en C 
	Desde el cmd nos dirijimos a la carpeta winutils y ejecutamos winutils.exe chmod 777 \tmp\hive (esta carpeta tmp al no existir, habrá que crearla previamente)

		CONFIGURANDO LAS VARIABLES DE ENTORNO

	Ahora debemos añadir las variables de entorno. 

	HADOOP_HOME ----> C:\winutils
	SPARK_HOME  ----> (ruta donde se haya descomprimido Spark)
	JAVA_HOME   ----> (ruta donde se haya instalado JAVA)
	Path -----------> %SPARK_HOME%\bin
	Path -----------> %JAVA_HOME%\bin
