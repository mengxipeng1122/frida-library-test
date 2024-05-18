# Frida-library-test

This repository demonstrates the utilization of a library within a frida-compile project.

## Library Compilation
To compile the library, navigate to the my-frida-project directory and execute the following commands:
```bash
cd my-frida-project
npm run build
npm pack
```

These commands will generate a package file located at `my-library/my-library-1.0.0.tgz`.

## Project Compilation
To compile the project, switch to the my-frida-project/ directory and execute the following commands:
```bash
cd my-frida-project/
npm install
npm install ../my-library/my-library-1.0.0.tgz
make
```

This will output a JavaScript file at `my-frida-project/_agent.js`.

# Note
It is crucial to employ frida-compile version 10, as opposed to the latest version, for this process.
