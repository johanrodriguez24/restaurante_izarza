# restaurante_izarza

Pasos para Configurar WordPress Localmente Usando XAMPP
Paso 1: Descargar e Instalar XAMPP
Descargar XAMPP:

Ve al sitio oficial de XAMPP: https://www.apachefriends.org/index.html.
Descarga la versión correspondiente a tu sistema operativo (Windows, macOS o Linux).
Instalar XAMPP:

Sigue las instrucciones del instalador para instalar XAMPP en tu computadora. No necesitas cambiar muchas opciones; puedes instalarlo con las configuraciones predeterminadas.
Paso 2: Configurar XAMPP
Iniciar XAMPP:

Una vez que XAMPP esté instalado, abre el Panel de Control de XAMPP.
Inicia los módulos Apache (servidor web) y MySQL (base de datos) haciendo clic en "Start" en ambos.
Verificar que Apache y MySQL estén Corriendo:

Abre tu navegador y escribe http://localhost/ en la barra de direcciones.
Deberías ver la página de bienvenida de XAMPP si todo está funcionando correctamente.
Paso 3: Descargar WordPress
Descargar WordPress:

Ve al sitio oficial de WordPress: https://es.wordpress.org/download/.
Descarga el archivo ZIP de WordPress.
Extraer WordPress:

Extrae el archivo ZIP de WordPress en la carpeta de XAMPP.
Ve a la carpeta donde instalaste XAMPP (por ejemplo, C:\xampp\htdocs\ en Windows) y crea una carpeta para tu proyecto, por ejemplo, restaurante.
Copia todos los archivos de WordPress extraídos en esa carpeta (C:\xampp\htdocs\restaurante).
Paso 4: Crear una Base de Datos para WordPress
Abrir phpMyAdmin:

En el navegador, ve a http://localhost/phpmyadmin/. Esto abrirá la herramienta phpMyAdmin, que te permite administrar bases de datos MySQL.
Crear una Nueva Base de Datos:

Haz clic en la pestaña Bases de datos.
Crea una nueva base de datos. Puedes llamarla, por ejemplo, wordpress_db.
Selecciona el cotejamiento utf8_general_ci para asegurarte de que tu base de datos soporte caracteres especiales.
Paso 5: Instalar WordPress
Iniciar la Instalación:

En el navegador, ve a http://localhost/restaurante (o la carpeta que creaste en htdocs).
Aparecerá la pantalla de instalación de WordPress.
Configurar la Conexión a la Base de Datos:

En la pantalla de instalación, WordPress te pedirá los datos de la base de datos:
Nombre de la base de datos: wordpress_db (o el nombre que le diste).
Nombre de usuario: root (por defecto en XAMPP).
Contraseña: Deja esto en blanco (por defecto en XAMPP).
Servidor de base de datos: localhost.
Prefijo de tabla: wp_ (puedes dejar el valor por defecto).
Completar la Instalación:

WordPress te pedirá información adicional, como el nombre del sitio, tu correo electrónico, y la creación de un usuario administrador. Completa estos datos y haz clic en Instalar WordPress.
Paso 6: Acceder al Panel de Administración de WordPress
Iniciar sesión en WordPress:
Una vez finalizada la instalación, puedes acceder al panel de administración de WordPress desde http://localhost/restaurante/wp-admin.
Inicia sesión con las credenciales que acabas de crear.
Crear el Tema Hijo y el Plugin Personalizado en Local
Una vez que WordPress esté corriendo en tu entorno local, puedes crear tu tema hijo y tu plugin personalizado tal como te expliqué anteriormente. Las rutas que mencioné ahora estarán dentro de la carpeta donde instalaste WordPress localmente:

Tema hijo:

Ve a C:\xampp\htdocs\restaurante\wp-content\themes\.
Crea la carpeta mi-tema-hijo y sigue los pasos para crear el archivo style.css y functions.php.
Plugin personalizado:

Ve a C:\xampp\htdocs\restaurante\wp-content\plugins\.
Crea la carpeta mi-plugin-backend y el archivo mi-plugin-backend.php con el código del plugin.
Acceder a la Base de Datos Localmente
Puedes interactuar con la base de datos local a través de phpMyAdmin, que está en http://localhost/phpmyadmin. Aquí es donde puedes ver, crear o editar tablas, y también puedes ejecutar consultas SQL.

Para interactuar desde el plugin, usarás $wpdb, como te mostré antes, que ya viene integrado con WordPress para hacer consultas SQL fácilmente.

Opcional: Instalar WordPress en Local con Local by Flywheel
Si prefieres una opción más sencilla que XAMPP, puedes usar una herramienta llamada Local by Flywheel. Es muy fácil de usar y te permite instalar WordPress localmente con un par de clics.

Descargar Local by Flywheel:

Ve al sitio oficial de Local by Flywheel: https://localwp.com/.
Descarga e instala la aplicación.
Crear un Nuevo Sitio de WordPress:

Abre Local by Flywheel.
Haz clic en Create a New Site y sigue las instrucciones para configurar tu instalación de WordPress local.
Local se encargará de todo (Apache, MySQL y PHP), y tendrás WordPress funcionando sin necesidad de configurar nada manualmente.
Conclusión
Ahora que tienes WordPress instalado localmente con XAMPP (o Local by Flywheel), puedes desarrollar tu sitio web en tu propio equipo sin necesidad de un servidor web en línea. Una vez terminado el desarrollo, podrás exportarlo a un hosting real.

Temas Hijos y Plugins Personalizados se gestionan igual que en un entorno de producción, pero todas las rutas ahora apuntarán a tu instalación local en XAMPP (C:\xampp\htdocs\restaurante\wp-content\themes\ y \plugins\).
¿Listo para comenzar a personalizar WordPress localmente o hay algo que no esté claro? ¡Déjame saber si necesitas más detalles!
Contraer
message.txt
6 KB
