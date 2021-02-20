# vercel-express

Vercel Express y UI Webapp ejemplo.

Demo - https://exprets.vercel.app/

- Primero clone el repositorio en un directorio local. Configure la línea de comando de vercel y ejecute el comando "vercel" para implementar el proyecto:

### Configurar e implementar con Vercel

```
$ npm install vercel -g
$ npm install
$ vercel
```

- Vercel generará un directorio ".vercel", no comparta nada de este.
- Después de la implementación, abra su URL así:
  - http://YOUR-VERCEL-APP-ID.vercel.app
  - Example: https://exprets.vercel.app/

### [app/index.js](./app/index.js)

- Si está usando TypeScript con node, cree su directorio de origen (usando una herramienta como la línea de comando "tsc" del paquete "typescript"), y envíe la salida a "app".
- Actualización package.json: "main": "app/index.js"

### [vercel.json](./vercel.json)

- Mapa de rutas API(/api/...) y rutas estáticas (UI) (/...).
- Variables de entorno - ejemplos:
  - ```$ vercel secrets add my-mongodb-uri mongodb+srv://<user>:<password>@clusteridxxx.mongodb.net/<database-name>?retryWrites=true```
  - agregue "env" a vercel.json ```{" env ": {" MONGODB_URI ":" @ my-mongodb-uri "},...```

¡Ahora tiene una aplicación web completa implementada en Internet usando Vercel!
¡Feliz codificación!
