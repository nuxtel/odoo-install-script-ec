<h3>Procedimiento de instalación</h3>
https://ventor.tech/odoo/odoo-installation-script/
1. **Descarga el script:**
``texto
clon git https://github.com/ventor-tech/odoo-install-script
```
2. **Modifique los parámetros como desee.**
Hay algunas cosas que puedes configurar, esta es la lista más utilizada:

- OE_USER - será el nombre de usuario para el usuario del sistema.
- OE_HOME - será el directorio de inicio del usuario del sistema.
- OE_VERSION - es la versión de Odoo a instalar, por ejemplo _10.0_ para Odoo V10.
- OE_INSTALL_DIR - es la ruta donde se instalará todo el entorno.
- OE_REPO - es la ruta donde se clonará odoo.
- INSTALL_WKHTMLTOPDF - configúrelo en _False_ si no desea instalarlo, si desea instalarlo debe configurarlo en _True_.
- OE_PORT - es el puerto donde debe ejecutarse Odoo, por ejemplo 8069.
- OE_NETRPC_PORT - es el puerto donde debe ejecutarse Odoo net-rpc, por ejemplo 8070.
- OE_LONGPOOL_PORT - es el puerto donde debe ejecutarse el pool largo de Odoo, por ejemplo 8070.
- IS_ENTERPRISE - instalará la versión Enterprise sobre la versión comunitaria si la configura como _True_, configúrela como _False_ si desea la versión comunitaria de Odoo.
- OE_SUPERADMIN - es la contraseña maestra para esta instalación de Odoo.
- OE_DB_PASSWORD - es la contraseña del usuario de postgres.
- OE_WORKERS - es el número de trabajadores de Odoo
- PG_VERSION - es una versión de postgresql instalada

3. **Conviértete en root**
```text
su
```
4. **Hacer que el script sea ejecutable**
```text
sudo chmod +x run.sh
```
5. **Ejecutar el script:**
```text
sudo ./run.sh
```
