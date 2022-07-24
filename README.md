## FileRun
FileRun es un sistema de software de alojamiento de archivos multiplataforma

## About

<p align="center">
<img src="https://github.com/JuanRodenas/Seafile/blob/main/seafile.png" />
</p>

FileRun es una aplicación basada en web de File Sync and Share autohospedada. Es un administrador de archivos basado en la web con todas las funciones con una interfaz de usuario fácil de usar.

### Documentación
<ul>
<li><p>Nos dirigimos a <code>/etc/hosts</code> y añadimos:</p></li>
<p><a href="https://github.com/filerun/docker">Github</a></p>
<p><a href="https://docs.filerun.com/docker">Documentation</a></p>
<p><a href="https://hub.docker.com/r/filerun/filerun/">Docker Image</a></p>

<sup>Para las CPU ARM64 (Raspberry Pi), utilice.</sup>
<p><a href="https://docs.filerun.com/docker-arm64">CPU ARM64 (Raspberry Pi)</a></p>
</ul>

## Files
- Descargamos el repositorio:
```
git clone "https://github.com/JuanRodenas/FileRun.git"
```
-Creamos carpeta en el directorio de persistencia:
```
mkdir shared
```

### Configuration
Sustituya las variables de entorno en `.env` por las suyas propias, y luego ejecute :

```bash
docker-compose up -d
```

Entonces debería poder acceder a la web-ui de FileRun con el `SEAFILE_ADMIN_EMAIL` y `SEAFILE_ADMIN_PASSWORD`.

## Update
Si quiere actualizar la imagen automáticamente con watchtower gracias a la siguiente etiqueta:

```yaml
  # Watchtower Update
  - "com.centurylinklabs.watchtower.enable=true"
```
