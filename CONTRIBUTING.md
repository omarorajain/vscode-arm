The extension is all TypeScript. It does not employ language server and language features are implemented directly.

### Setup
1. Install [VS Code](https://code.visualstudio.com/download).
2. Fork and clone the [repo](https://github.com/omarorajain/vscode-arm).
3. Install [node.js](https://nodejs.org/en)
4. Open command prompt.
5. From the cloned root run `npm install`.
6. Run `npm run build`.
7. Run VS Code.
8. Install extensions: 
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Jest](https://marketplace.visualstudio.com/items?itemName=Orta.vscode-jest)

9. Open folder in VS Code.
10. You should be able to run the extension and tests from VS Code.

### Coding guidelines
Nothing special, standard TypeScript conventions. For formatting - tab size is 2, spaces only. Test runner is [Jest](https://jestjs.io/).

### Instruction documentation
[Instruction documentation](https://github.com/MikhailArkhipov/vscode-arm/tree/main/src/instruction_sets) for A32 and A64 was generated from ARM sources, downloads are [here](https://developer.arm.com/downloads/-/exploration-tools). This documentation is short version that is used in hover and completions. Generator code is in a [separate repo](https://github.com/MikhailArkhipov/arm-doc-converter). 

The extension can open full instruction documentation in browser contained in HTML files from [ARM documentation archives](https://developer.arm.com/downloads/-/exploration-tools) unpacked into another [separate repo](https://github.com/MikhailArkhipov/ARM-doc).

### Directives documentation
Fetched directly from GAS/GCC Web site. No local caching is implemented at the moment. See [documentation.ts](https://github.com/MikhailArkhipov/vscode-arm/blob/main/src/documentation/documentation.ts)