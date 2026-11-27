Preguntas de reflexión
1. ¿Qué podía hacer el usuario justo después de crearlo, antes de adjuntarle una política? ¿Por qué?
R/ No podria realizar acciónes sobre los servicios de AWS porque al momento de crear un usuario IAM no recibe permisos automaticamente por eso no tiene permiso de acceder a los recursos.

2. En el error del paso 13, ¿qué tres datos te dice el mensaje?
R/los datod que veo son: la identidad (admin-isaac-).
la acción denegada (iam:ListAccessKeys.)
el recurso que indica que usuario intenta realizar la acción 


3. ¿Por qué cambió el Arn al renombrar el usuario?
R/ Porque el ARN identifica al usuario mediante su ruta y nombre. Cuando cambiamos el nombre de jesus a david, AWS actualiza el ARN para reflejar el nuevo nombre

4. ¿Por qué AWS obliga a borrar las llaves antes de borrar el usuario?
R/Porque las llaves de acceso son credenciales que permiten conectarse a AWS mediante herramientas como AWS CLI o aplicaciones.

5. ¿Qué pasaría si le hubieras dado AdministratorAccess en vez de solo lectura? ¿En qué caso real estaría justificado?
R/El usuario tendría permisos administrativos muy amplios sobre los servicios de AWS, dependiendo de las restricciones adicionales de la cuenta.