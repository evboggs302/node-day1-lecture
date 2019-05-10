## Node

- Student can create an index.js file
- Student can run a javascript file using node
- Student can run a javascript file using nodemon
- Student can describe that node is the V8 javascript engine
- Student can require and use other files in node

## Servers

- Student can describe the role of servers in a client-server model
- Student can identify the parts of code that listen to external requests

## NPM

- Student can npm init
- Student can npm install
- Student can npm install --save
- Student can describe the role of a package.json file
- Student can describe the purpose of the node_modules folder
- Student can .gitignore node_modules

## Express

- Student can install and require express
- Student can start a basic express server by creating an app and listening on a port
- Student can write the handler function with the correct parameters req, res and next
- Student can access url parameters on req.params
- Student can set up an endpoint path to expect multiple params
- Student can use req.query
- Student can send data back with res.send and res.json
- Student can set a status code with res.status

---

**NPM:**

- 'Node Package Manager'
- a giant code base for developers to make features, tools, utilities available to general public.
- a community of people that have given code to be given

**YARN:**

- made by Facebook
- download same packages as NPM but was initially a ton faster than NPM

**Package.json:**

- package.json is a config file for our applicaiton with instructions on dependencies to download, and how to node should run for application.

https://docs.npmjs.com/files/package.json

**.GITIGNORE:**

- a file listing other file/directory names that should NOT be pushed to GitHub.

  - node modules
  - .env files.
  - anything you don't want on GitHub

**Server:**

- a computer/device that provides a service to another computer
- in general for us --> a webserver is a program that can handle incoming reqs and respond accordingly.
- manages access to a centralized resource:

  - todays centralized resource: `data.json`

**Client:**

- a computer/program that accesses a service made available by a server

**SERVER INSTRUCTIONS:**

    mkdir server
    touch index.js && .gitignore
    npm init -y
    add node_modules => .gitignore
    npm i express
    in index.js =>
        require express
        declare var app = express()
        declare port #
        app.listen => port
        declare end point
        method -- .get
        path -- '/api....'
        handler function -- (req, res, next) => data to send
        test in browser

**Params:**

- typically stands for a particular resource
- looks liek a normal path on the front end, but denoted with a ';'

```js
app.get("/app/:id");
```

(accessing params in fucntion)

```js
req.params.id;
```

**Querys:**

- ways we would like to manipulate the accessed data. denoted with a '?'

front end example:

```js
"https://localhost:4000/api/students?name=josh";
```

access query in endpoint function handler:

```js
req.query.name;
```
