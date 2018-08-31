- [Instalación con drush](#instalaci%C3%B3n-con-drush)

# Instalación con drush

> Nota: Tiene que ser drush versión 8
0. verificar drush con `drush status`
![](./assets/img/drushStatus.png)
1. Creamos un host
2. Abrimos la consola y nos ubicamos en la carpeta en donde trabajaremos, `htdocs?` de xampp
3. Descargamos la última versión de drupal con el comando `drush dl` y esperamos a que descargue...
4. Renombramos la carpeta descargada con el comando `mv` ejemplo `mv drupal-8.x/ nombredelproyecto` e ingresamos a la carpeta
5. Ejecutamos el comando de instalación por medio de drush `drush si --db-url=mysql://root:password@localhost/nombreBaseDeDatos -y` y esperamos a que se instale...
6. Una vez terminada la instalación, podemos ver como se crearon los archivos de configuración en la carpeta `/sites/default` estos son los archivos: `default.services.yml`, `default.settings.php`, `settings` ademas de la carpeta `files/` que sera donde se almacenarán nuestros archivos.
7. Ingresamos el comando para cambiar el password de admin `drush upwd admin --password="contraseñaNueva"`
8. Accedemos a nuestro host y listo ya tenemos drupal para trabajar...

Para más info sobre los comandos: [drush 8.x](https://drushcommands.com/drush-8x/)

[Ir al inicio](./README.md)
