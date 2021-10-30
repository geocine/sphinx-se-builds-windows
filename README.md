<h1 align="center">
  <br>
  <a href="https://github.com/geocine/phaser3-rollup-typescript#readme"><img src="https://i.imgur.com/8MkldPt.png" alt="header" width="600"/></a>
  <br>
  Sphinx SE Builds for Windows
  <br>
</h1>


Sphinx SE build for MySQL Windows. Pre-compiled sphinx storage engine binaries for MySQL

### How to use

1. Download appropriate **ha_sphinx.dll**
2. Paste **ha_sphinx.dll** file to `mysql/lib/plugin`
3. Login to mysql console

		mysql -u <username> -p

4. Install plugin

		INSTALL PLUGIN sphinx SONAME "ha_sphinx.dll";

5. Still from mysql console execute show engines. It should show sphinx if you have installed it successfully

		show engines;
5. If you want to uninstall, here is how to do it.

		UNINSTALL PLUGIN sphinx;

