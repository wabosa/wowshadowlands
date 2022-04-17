# wowshadowlands
Build your own World Of Warcraft Blizlike Shadowlands Server




1.DESCARGAS:
Rich (BB code):
Repack Shadowlands: TrinityCore rev. 505bf6903a14+ 2022-03-23 Probado y trabajando en la versión 9.2.0 (42698)

Parche del cliente: Arctium WoW Client Launcher

Contraseña para descomprimir: www.wowcreador.com

2.EXTRAER LOS MAPAS
Dentro de la carpeta Extractores, copia los 5 archivos que están ahí y pégalos en la carpeta WoW /_retail_/ PEGA AQUI. Después ejecuta el archivo llamado extractor.bat se abrirá una consola y pondrás un 4, presionas ENTRER dos veces y empezará a extraer todos los mapas. El proceso puede tardar entre 2 a 8 horas según las especificaciones de tu computadora. Una vez que termine la consola, copia las nuevas carpetas que fueron generadas y las pegas en la carpeta del repack.

Extraer los mapas manualmente, este es el orden de ejecutarlos:
mapextractor
vmap4extractor
vmap4assembler
mmaps_generator
3.CREAR BASES DE DATOS
En caso que no tengas ninguna base de datos creada, ejecuta este codigo en tu editor de base de datos para crear las tres DB al mismo tiempo:
SQL:
GRANT USAGE ON * . * TO 'trinity'@'localhost' IDENTIFIED BY 'trinity' WITH MAX_QUERIES_PER_HOUR 0 MAX_CONNECTIONS_PER_HOUR 0 MAX_UPDATES_PER_HOUR 0 ;

CREATE DATABASE `world` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;

CREATE DATABASE `characters` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;

CREATE DATABASE `auth` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;

CREATE DATABASE `hotfixes` DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

GRANT ALL PRIVILEGES ON `world` . * TO 'trinity'@'localhost' WITH GRANT OPTION;

GRANT ALL PRIVILEGES ON `characters` . * TO 'trinity'@'localhost' WITH GRANT OPTION;

GRANT ALL PRIVILEGES ON `auth` . * TO 'trinity'@'localhost' WITH GRANT OPTION;

GRANT ALL PRIVILEGES ON `hotfixes` . * TO 'trinity'@'localhost' WITH GRANT OPTION;


4.CREAR CUENTA DESDE LA CONSOLA:
En la consola worldserver escribe este código de ejemplo para crear una cuenta: bnetaccount create wowcreador@wowcreador 123456
Establecer cuenta GM: account set gmlevel 1#1 3 -1
