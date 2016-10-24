Para corregir una falla en el uso del Plugin Cobertura, se realiza los siguientes ajustes:
- En la configuración del proyecto en Jenkins, en la sección "Ejecutar tareas 'maven' de nivel superior", con la versión Maven 3.3.9 se define el Goal siguiente: 
	javadoc:javadoc cobertura:cobertura -Dcobertura.report.format=xml
- Se ajusta el archivo pom.xml del proyecto game-of-life en el repo local eliminando la línea <skip>true</skip> del plugin maven-surefire plugin.  Actualizar dicho cambio en el repositorio GitHub.
	
