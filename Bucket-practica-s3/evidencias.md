1. ¿Por qué el nombre de tu bucket tuvo que ser distinto al de tus compañeros si cada uno tiene su propia cuenta?
R/Porque los nombres de los buckets son unicos a nivel global.
2. El usuario del paso 21 pudo leer un archivo, pero en el paso 22 no pudo ver la lista. ¿Qué acción le faltaba en la política?
R/le faltaba el permiso s3:ListBucket, que permite listar el contenido de bucket.
3. En la política, ¿qué significa el /* al final del Resource? ¿Qué pasaría si se quitara?
R/el /* indica que el permiso se aplica a todos los objetos que están dentro del bucket.
4. ¿En qué se diferencia compartir un archivo con un enlace temporal de hacer público el bucket?
R/ la diferencia es que un enlace temporal tienes que acceder a un archivo en especifico pero un lazo de tiempo determinado y bajos las condiciones de la url y en cambio en hacerlo publico permite que cualquier persona acceda a los objetos expuestos.
5. Según el modelo de responsabilidad compartida, si alguien deja un bucket público con datos de clientes, ¿de quién es la responsabilidad?
R/La responsabilidad es del cliente que administra la cuenta de AWS, porque debe configurar correctamente los permisos, proteger los datos y controlar quién puede acceder a ellos.
