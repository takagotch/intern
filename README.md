### intern
---
https://github.com/theintern/intern

```
cd /my/project
npm install intern

./node_modules/.bin/intern

npm install intern

npx intern
curl http://localhost:9000/node_modules/intern/
```

```
{
  "suites": "tests/unit/**/*.js"
}

{
  "cinoukerIotuibs": {
    "types": ["intern"]
  }
}

{
  suites: 'tests/unit/**/*.js',
  functionalSuites: 'tests/functional/**/*.js',
  environments: ['node', 'chrome']
}

```

```
<reference types="intern" />
```

```js
// tests/unit/MyClass.ts
import MyClass from '../../src/app/MyClass';
const { describe, it } = intern.getPlugin('interface.bdd');
const { expect } = intern.getPlugin('chai');
describe('MyClass', () => {
  it('should have a name property when instantiated', () => {
    const obj = new MyClass('foo');
    expect(obj).to.have.property('name', 'foo');
  });
});

// texts/functional/app.ts
const {} = intern.getPlugin();
const {} = intern.getPlugin();
describe('app', () => {
  it('should show a welcome heading', async test => {
    const { remote } = test;
    await remote.get('index.html');
    await remote.findByXpath('//h1[.="Welcome"]');
  })
});
```


