1. En el paso 20, la instancia responde con un rol y no con un usuario. ¿De dónde sacó esas credenciales si nunca corriste `aws configure`?

R/ Porque la instancia obtuvo las credenciales automaticamente mediante AIM.

2. ¿Por qué el puerto 80 puede estar abierto a todo internet y el 22 no?

R/Porque el puerto 80 se utiliza para permitir que cualquier persona pueda acceder a la página web mediante HTTP.

3. La instancia pudo leer `reporte.txt` pero no listar el bucket. ¿Dónde se decidió eso?

R/se decidió en la política IAM asociada al rol `ec2-lector-s3`. Esta política permite la acción `s3:GetObject`, que permite leer archivos, pero no permite `s3:ListBucket`, que es necesaria para listar el contenido del bucket.

4. ¿Por qué cambió la IP pública al apagar y encender? ¿Qué problema traería eso en un sitio web real?

R/Porque AWS libera la dirección IP pública dinámica cuando detenemos una instancia y normalmente asigna otra cuando vuelve a iniciarse.

5. EC2 es infraestructura como servicio (IaaS). En esta práctica, ¿qué fue responsabilidad tuya y qué fue responsabilidad de AWS?

R/Mis responsabilidades:

configuara y administrar la instancia EC2.

Elegir el sistema operativo y el tipo de instancia.

Crear el Security Group y configurar sus reglas.

Responsabilidades de AWS:

Proporcionar la infraestructura física.

Proporcionar el servicio EC2 y sus recursos virtualizados.

6. Para tener este mismo servidor en una oficina, sin la nube, ¿qué habrías tenido que comprar y configurar?

R/Habría necesitado comprar un servidor físico, memoria RAM, almacenamiento, procesador, equipos de red, router  y una conexión a Internet.

También habría tenido que instalar y configurar Linux, Apache, las reglas de seguridad, las direcciones IP, los usuarios, los permisos y los servicios de mantenimiento y copias de seguridad.
