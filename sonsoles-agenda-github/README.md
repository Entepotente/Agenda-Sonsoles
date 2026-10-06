# Sonsoles Agenda — archivos para crear el APK

Este proyecto convierte la agenda web incluida en `www/index.html` en una aplicación Android usando Capacitor. GitHub Actions compila el APK en la nube; no hace falta instalar Node.js ni Android Studio en tu ordenador.

## Subirlo a GitHub

1. Crea un repositorio nuevo en GitHub.
2. Descomprime este paquete y sube **el contenido** de esta carpeta al repositorio (deben quedar visibles `package.json`, `capacitor.config.json`, `www/` y `.github/` en la raíz).
3. En GitHub, abre la pestaña **Actions** y permite los flujos de trabajo si GitHub lo solicita.
4. El flujo se ejecuta al subir cambios a `main` o `master`. También puedes iniciarlo desde **Actions → Crear APK Android → Run workflow**.
5. Cuando termine correctamente, abre esa ejecución, baja a **Artifacts** y descarga **Sonsoles-Agenda-APK**. Dentro está `app-debug.apk`, que puedes pasar a un móvil Android e instalar.

## Importante

El APK de este flujo es de depuración, adecuado para instalar y probar en un móvil. Para publicar en Google Play hace falta generar una versión de lanzamiento y firmarla con una clave propia.

La agenda es una primera maqueta: las tareas se pueden completar y añadir durante el uso actual; todavía no se guardan de forma permanente entre sesiones y no envía notificaciones reales.
