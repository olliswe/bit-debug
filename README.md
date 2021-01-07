Bootstrapped using `create-react-app`

To reproduce bug:

clone repo

run `bit import bit.envs/compilers/react-typescript@3.1.64 -c`

run `bit tag app`

You should see the following error:

```
App.tsx:2:8 - error TS1192: Module '"/private/var/folders/ry/fb0749q11w1cnktj1fbhgh0m0000gn/T/bit/capsule-85517/node_modules/components/HelloWorld"' has no default export.

2 import HelloWorld from "components/HelloWorld";
         ~~~~~~~~~~

  node_modules/components/HelloWorld.tsx:1:1
    1 export * from '../../components/HelloWorld';
      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    'export *' does not re-export a default.


Found 1 error.


error: bit failed to build app with the following exception:
Command failed with exit code 2: /Users/oliver/bit-debug/.git/bit/components/compilers/react-typescript/bit.envs/3.1.64/components/.dependencies/compilers/typescript/bit.envs/3.1.49/node_modules/typescript/bin/tsc --declaration
Error: Command failed with exit code 2: /Users/oliver/bit-debug/.git/bit/components/compilers/react-typescript/bit.envs/3.1.64/components/.dependencies/compilers/typescript/bit.envs/3.1.49/node_modules/typescript/bin/tsc --declaration
    at makeError (/Users/oliver/bit-debug/.git/bit/components/compilers/react-typescript/bit.envs/3.1.64/components/.dependencies/compilers/typescript/bit.envs/3.1.49/node_modules/execa/lib/error.js:59:11)
    at handlePromise (/Users/oliver/bit-debug/.git/bit/components/compilers/react-typescript/bit.envs/3.1.64/components/.dependencies/compilers/typescript/bit.envs/3.1.49/node_modules/execa/index.js:114:26)
    at process._tickCallback (internal/process/next_tick.js:68:7)

```
