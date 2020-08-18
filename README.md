# vscode-ts-debug-failure

Open this folder in VSCode, and push F5 to start debugger.

And then got the message:

```
node ./src/app.ts
Debugger listening on ws://127.0.0.1:39565/f914f928-b8af-4bda-bf0d-3db1a057327b
For help, see: https://nodejs.org/en/docs/inspector
Debugger attached.
(node:5155) Warning: To load an ES module, set "type": "module" in the package.json or use the .mjs extension.
Debugger listening on ws://127.0.0.1:39565/f914f928-b8af-4bda-bf0d-3db1a057327b
For help, see: https://nodejs.org/en/docs/inspector
/home/angus/projects/fenying/vscode-debug-test/src/app.ts:1
import { add } from './lib';
^^^^^^

SyntaxError: Cannot use import statement outside a module
    at wrapSafe (internal/modules/cjs/loader.js:1054:16)
    at Module._compile (internal/modules/cjs/loader.js:1102:27)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:1158:10)
    at Module.load (internal/modules/cjs/loader.js:986:32)
    at Function.Module._load (internal/modules/cjs/loader.js:879:14)
    at Function.executeUserEntryPoint [as runMain] (internal/modules/run_main.js:71:12)
    at internal/main/run_main_module.js:17:47
Process exited with code 1
(node:5155) Warning: To load an ES module, set "type": "module" in the package.json or use the .mjs extension.
```

However, see the [launch.json](./.vscode/launch.json), it's configured for TS correctly.
