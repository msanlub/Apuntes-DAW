  ## Acceso e información del docker
  
  `docker start nombre_contenedor
	Iniciamos un contenedor ya creado.
	
  `docker exec nombre_contenedor comando
	  ejemplo: `docker exec -dit segundo-cgi bash
	  Para entrar en el contenedor y acceder a su información.
	  Una vez dentro puedo acceder a cuando se ha entrado en la web, por ejemplo, con la siguiente ruta:
		  `cat /var/log/nginx/access.log`

