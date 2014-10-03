# sphinx-se-builds

Sphinx SE build for MySQL Windows. Pre-compiled sphinx storage engine binaries for MySQL

### How to use

1. Download appropriate **ha_sphinx.dll**
2. Paste **ha_sphinx.dll** file to `mysql/lib/plugin`
3. Login to mysql console

		mysql -u r<username> -p

4. Install plugin

		INSTALL PLUGIN sphinx SONAME "ha_sphinx.dll"

5. Still from mysql console execute show engines. It should show sphinx if you have installed it successfully

		show engines;
5. If you want to uninstall, here is how to do it.

		UNINSTALL PLUGIN sphinx

