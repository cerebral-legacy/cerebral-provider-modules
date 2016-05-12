# cerebral-provider-modules
Modules pattern for Cerebral

```js
function myAction({modules, module}) {
  module // Current module
  module.services // Services of the module
  module.state // State on the module
  module.meta // Meta returned from module

  modules // All modules, with services, state, and meta
}
```
