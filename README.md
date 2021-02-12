# vercel-express

Vercel Express y UI Webapp ejemplo.

Demo - https://exprets.vercel.app/

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

- Si está utilizando TypeScript, cree su directorio de origen, salida a "app"
- Actualización package.json: "main": "app/index.js"

### [vercel.json](./vercel.json)

- Mapa de rutas API(/api/...) y rutas estáticas (UI) (/...).
- Variables de entorno - ejemplos:
  - ```$ vercel secrets add my-mongodb-uri mongodb+srv://<user>:<password>@clusteridxxx.mongodb.net/<database-name>?retryWrites=true```
  - agregue "env" a vercel.json ```{" env ": {" MONGODB_URI ":" @ my-mongodb-uri "},...```
