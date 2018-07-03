# TypeScript Basics

## Requirements
Recommended: 
* node.js 8.11.3 LTS + npm installed
* An IDE with TypeScript support, e.g. Jetbrains WebStorm

## Project setup
In order to have a minimal development environment for using TypeScript, execute the following commands 
on the command line:

* To create node project and package.json
```bash
npm init
```
* Install dependencies
```bash
npm install typescript --save
# short form
npm i typescript -S
```
* Edit package.json and add tsc and start script
```json
{
  "name": "typescript-basics",
  "version": "1.0.0",
  "description": "",
  "private": true,
  "main": "index.js",
  "scripts": {
    "tsc": "tsc",
    "start": "npm run tsc"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "dependencies": {
    "typescript": "^2.9.2"
  }
}
```
* Initialize TypeScript project
```bash
npm run tsc -- --init
```

* Create source folder and index.ts file with "Hello World" output (works on UNIX command line)
```bash
mkdir src
touch src/index.ts
echo "console.log('Hello World!');" > src/index.ts
```

* Build it
```bash
npm run start
```

* Run it
```bash
node src/index.js
```