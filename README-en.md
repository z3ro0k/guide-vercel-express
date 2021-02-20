# vercel-express

Vercel Express y UI Webapp example.

Demo - https://exprets.vercel.app/

First, clone the above repository to a local directory. Set up vercel command line and run “vercel” command to deploy the project:

### Set up & Deploy with Vercel

```
$ npm install vercel -g
$ npm install
$ vercel
```

- Vercel will generate a “.vercel” directory, don’t share or commit this one.
- After deploying, open your URL that looks like this:
  - http://YOUR-VERCEL-APP-ID.vercel.app
  - Example: https://exprets.vercel.app/
  ### [app/index.js](./app/index.js)

- If you’re using Typescript with node, build your source directory (using a tool like “tsc” command line from “typescript” package), output to “app”.
- Update package.json: “main”: “app/index.js”

### [vercel.json](./vercel.json)

- Map API routes (/api/…) and static (UI) routes (/…).
- Environment variables - examples:
  - ```$vercel secrets add my-mongodb-uri mongodb+srv://<user>:<password>@clusteridxxx.mongodb.net/<database-name>?retryWrites=true```
  - add "env" to vercel.json ```{" env ": {" MONGODB_URI ":" @ my-mongodb-uri "},...```

You now have a complete web application deployed on the internet using Vercel!
Happy coding!
