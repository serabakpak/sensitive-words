# Example
```shell
$ npm i sensitive-words --save
```

```js
const { sensitiveWords } = require('sensitive-words');

// 2015 modules
import { sensitiveWords } from 'sensitive-words');

const filtered = sensitiveWords(
  'The new Apple macbook Pro will have a touchbar.',
  ['pro', 'touchbar']
);

console.log(filtered);
// The new apple macbook *** will have a ***.
```

# Scripts
`npm run build` = `babel src -d build` (compiles src dir --> build dir)

`npm run dev` = `watch 'npm run build' src`, (run build whenever src dir changes)

# Misc
`prepublish` = `npm run build` (this ensures that we have the latest build every time we run `npm publish`)
