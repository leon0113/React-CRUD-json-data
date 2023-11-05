# render-json-server


**Step 1** -   Create git repository

**Step 2** - Clone it on your device

**Step 3** - Add package.json by using this command `npm init -y`

**Step 4** - Install some dependency by using this command `npm i json-server cors json-serve` and add ` "start": "node index.js" ` in script 

**Step 6** - Create index.js file copy the code from my GitHub repository

```javaScript
const jsonServer = require("json-server"); // importing json-server library
const server = jsonServer.create();
const router = jsonServer.router("db.json");
const middlewares = jsonServer.defaults();
const port = process.env.PORT || 8080; //  chose port from here like 8080, 3001

server.use(middlewares);
server.use(router);

server.listen(port);

```

**Step 7** - Add db.json and add .gitignore file


After all this steps are completed use this command to push the code in your Github account.

`git add .`

`git commit -m "Your message"`

`git push origin main`

