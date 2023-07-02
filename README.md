# How to create node project

## Description

Commands to create a nodeJS project from scratch

## Commands

1. Create a folder with your project name and then access that folder in terminal

2. Init node project run below command

```bash
npm init -y
```

3. Create _.npmrc_ file and add in the file

```code
save-exact=true
```

4. Create _.env_ file and _.env.example_ file

5. Install [dotenv](https://www.npmjs.com/package/dotenv) to use environment variables inside the project

```bash
npm i dotenv
```

6. Create a _env_ folder inside _src_ folder (src/env) and add the file _index.ts_ there we will load our env variables

7. Install [zod](https://www.npmjs.com/package/zod) to help us validate our schemas

```bash
npm i zod
```  

8. Install [typescript](https://www.npmjs.com/package/typescript) (for typescript projects), I will use _npm_ for my projects
   I will install too [tsx](https://www.npmjs.com/package/tsx) and [tsup](https://www.npmjs.com/package/tsup), both will help us in develop and production environment

```bash
npm i typescript @types/node tsx tsup -D
```

9. Create tsconfig

```bash
npx tsc --init
```

9.1 Inside tsconfig change target to ES2020

![image](https://github.com/jhonatasmatos/how-to-create-node-project/assets/16242029/5cfce3cc-92be-4262-89e4-c147c4c16030)

10. Install [fastify](https://www.npmjs.com/package/fastify)

```bash
npm i fastify
```

11. Create .gitignore file and add there node_modules, build and after other files

12. Create _src_ folder and inside create _server.ts_ file

13. Create below scripts inside _package.json_

```json
"scripts": {
    "dev": "tsx watch src/server.ts",
    "start": "node build/server.js",
    "build": "tsup src --out-dir build"
  },
```

14. Instal [eslint](https://www.npmjs.com/package/eslint) to do lint

```bash
npm i eslint -D
```

14.1 Init eslint

```bash
npx eslint --init
```

14.2 Answer the questions according to your preference

![image](https://github.com/jhonatasmatos/how-to-create-node-project/assets/16242029/f5ece3c3-0be8-4a25-962e-c82eb4b5d858)
