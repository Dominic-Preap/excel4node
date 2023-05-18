# Use cases:
## Use case 1: 
After npm i excel4node in your typescript project, find a good location inside your project files. I used src/utils/modules
```bash
touch excel4node.js
```
```javascript
// eslint-disable-next-line @typescript-eslint/no-var-requires
const xl = require('excel4node');
module.exports = xl;
```
After this, download the only file of this repository or copy paste it in: src/utils/modules

```typescript
import {Workbook, Style, Worksheet} from '../../utils/modules/excel4node.js'
```

Now you can use excel4node with typescript