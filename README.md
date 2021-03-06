# @coreui/vue + Vue ACL

[![Npm badge](https://img.shields.io/npm/v/svdesignti-coreui-vue-acl.svg)][npm]
![Vue](https://img.shields.io/badge/Vue-^2.5.13-brightgreen.svg)

[npm]: https://www.npmjs.com/package/svdesignti-coreui-vue-acl

> A [@coreui/vue](https://coreui.io/vue) `v2` library project

for use with [CoreUI](https://coreui.io/vue/) `v2` Open Source Bootstrap Admin Template

## Installation
```
npm install svdesignti-coreui-vue-acl
```
svdesignti-coreui-vue-acl can be used as a module in both CommonJS and ES modular environments.

When in non-modular environment, svdesignti-coreui-vue-acl will register all the components to vue by itself.</p>

### ES6 
```js
//
// You can register a component manually
//
import { Switch } from 'svdesignti-coreui-vue-acl';

export default {
  ...
  components: {
    Switch
  },
  ...
};

//
// or register the whole module with vue
//
import ModuleLibrary from 'svdesignti-coreui-vue-acl';

// Install this library
Vue.use(ModuleLibrary);
```

## Changelog

See the GitHub [release history](https://github.com/coreui/coreui-vue/releases).

## Contributing

See [CONTRIBUTING.md](.github/CONTRIBUTING.md).
