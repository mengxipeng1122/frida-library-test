# Frida-library-test

This repository demonstrates the utilization of a library within a frida-compile project.

## Library Compilation
To compile the library, navigate to the my-library directory and execute the following commands:
```bash
cd my-library
make
```

These commands will generate a package file located at `my-library/my-library-1.0.0.tgz`.

## Project Compilation
To compile the project, switch to the my-frida-project/ directory and execute the following commands:
```bash
cd my-frida-project/
npm install
npm install ../my-library
make
```

This will output a JavaScript file at `my-frida-project/_agent.js`.

