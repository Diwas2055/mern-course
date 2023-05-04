# Complete MERN Beginner Course [2023]

- Full-stack MERN app with React, Node, Express, MongoDB Atlas, and TypeScript


## Creating Backend

```bash
# creating a folder called `backend`
mkdir backend
# navigate and change the working directory to `backend` folder
cd backend
# `npm init` used to set up a new or existing npm package and the `-y` flag when passed to NPM commands tells the generator to use the defaults instead of asking questions
npm init -y
```
### Installing Dependencies 

```bash
npm install --save-dev typescript  # install typescript 

# npm install express 
# or
npm i express # Express is a framework for node.js

npm i --save-dev @types/express # `TypeScript` definitions for `Express` framework

npm i --save-dev nodemon # nodemon is a tool that helps develop Node.js based applications by automatically restarting the node application when file changes in the directory are detected.

npm i -D ts-node # ts-node is a TypeScript execution engine and REPL for Node.js.


npm i -D eslint # ESLint is a tool for identifying and reporting on patterns found in ECMAScript/JavaScript code.

npx eslint --init # configure ESLint
```
> Note : Dependencies are the packages are used for our project
- There are two types of `Dependencies`:

    - `Normal Dependencies`
    - `Dev Dependencies` ("--save-dev","-D") = They are those packages that are not needed in production. They are only needed while creating a project.


### Typescript Configuration as we are using typescript packages 

- When we install the typescript packages it doesn't create a typescript config `file`

```bash
npx tsc --init
```

> Note: `NPM` is a package manager used to install, delete, and update Javascript packages on your machine. `NPX` is a package executer, and it is used to execute javascript packages directly, without installing them.

### To run the Typescript File in node.js 
- We need to convert the typescript file into js file 
```bash
npx tsc
```
> Note : It optimize the typescript file into js file 


### Run the node

```js
node server.js
```

### Update Config of Typescript for specifying the folder after compiling the typescript file into js file

- open `tsconfig.json`
- search for `outDir` and uncomment the line
- Now add the path where you want store the complied file


### For dynamic watch the change folder and auto compile the file

```bash
npx nodemon src/server.ts
```