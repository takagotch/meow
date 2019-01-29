### meow
---
https://github.com/sindresorhus/meow

```
npm install meow
./foo-app.js unicorns --rainbow
```

```js
#!/usr/bin/env node
'use strict';
const meow = require('meow');
const foo = require('.');
const cli = meow(`
  Usage 
    $ foo <input>
  Options
    --rainbow, -r Include a rainbow
  Examples
    $ foo unicorns --rainbow
`, {
  flags: {
    rainbow: {
      type: 'boolean',
      alias: 'r'
    }
  }
});

flasg: {
  unicorn: {
    type: 'string',
    alias: 'u',
    default: 'rainbow'
  }
}

const cli = meow(`

`, {
  booleanDefault: undefined,
  flags: {
    rainbow: {
      type: 'bollean',
      default: true,
      alias: 'r'
    },
    unicorn: {
      type: 'boolean',
      default: false,
      alias: 'u'
    },
    cake: {
      type: 'boolean',
    }
  }
});
```

```
```


