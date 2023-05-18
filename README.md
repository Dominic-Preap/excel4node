# excel4node

> ⚠️ If you come across any missing features or typing errors, please create PR and I will review it. Or maybe convince the author to officially include typing. Thank you.

A Typescript interface for [excel4node](https://github.com/advisr-io/excel4node).

## Usage

```sh
npm i excel4node
yarn add excel4node
```

After installing the library in your project, create a new typing file generally at the root of the project. Copy everything [inside](https://github.com/Dominic-Preap/excel4node/blob/master/typings/excel4node.d.ts) and paste to your file.

```sh
touch typings/excel4node.d.ts
```

```sh
•
├── 📁src                  # Your main source code
├── 📁typings              # Typings folder here
│   └── 📄excel4node.d.ts  # Create typing file here
├── 📄tsconfig.json        # Assuming you have a typescript project
```

If you have a Typescript project, you need to update your config in `tsconfig.json` by adding a glob pattern.

```json
{
  "compilerOptions": {},
  "include": ["src/**/*", "typings/**/*.ts"] // <-- Including glob pattern here
}
```

Now you can use `excel4node` with typescript

```typescript
import { Workbook, Style, Worksheet } from "excel4node";

// Create a new instance of a Workbook class
const wb = new Workbook();

// Add Worksheets to the workbook
wb.addWorksheet('Sheet 1');
wb.write('file.xlsx');
```
