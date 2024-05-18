# Frida-library-test

This repository demostrated how to use a library in a frida-compile project.

## Compiling library
```bash
cd my-frida-project
npm run build
npm pack
```
This command will output a package file at  `my-library/my-library-1.0.0.tgz`

## Compiling project
```bash
cd my-frida-project/
npm install
make
```
This command will output a .js at `my-frida-project/_agent.js`

# Note
The key point is use frida-compile V10, not use the lastest version. 


