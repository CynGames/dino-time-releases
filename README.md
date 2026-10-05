# Dino Time · releases

Instaladores firmados de Dino Time. El código vive en el repo privado `CynGames/dino-time`.

- **Instalar:** bajá `DinoTime_x.y.z_x64-setup.exe` de la [última release](https://github.com/CynGames/dino-time-releases/releases/latest).
- **Actualizar:** la app busca `latest.json` de la última release y se actualiza con un clic. Tus datos (`%APPDATA%\DinoTime`) no se tocan.

## Publicar una versión

Actions → **Publicar versión de Dino Time** → *Run workflow* con la versión (`1.0.1`) y las novedades.

Secretos del repo:

| Secreto | Qué es |
| --- | --- |
| `SOURCE_DEPLOY_KEY` | Clave SSH privada; su pública es una deploy key de solo lectura en `CynGames/dino-time`. |
| `TAURI_SIGNING_PRIVATE_KEY` | Clave minisign del updater (la pública está en `tauri.conf.json`). |
| `TAURI_SIGNING_PRIVATE_KEY_PASSWORD` | Opcional: contraseña de esa clave (la actual no tiene, así que no está cargado). |
