# cerebral-provider-modules
Modules pattern for Cerebral

`npm install cerebral-provider-modules`

```js
import ModulesProvider from 'cerebral-provider-modules';

(controller || module).addContextProvider(ModulesProvider);
```

```js
function SomeAction({module, modules}) {
  module.state.set('foo', 'bar');
  module.services.foo();
  module.meta // {path,name, ...}
  
  modules.someOtherModule.meta // {path,name, ...}
  modules.someOtherModule.state('foo', 'bar');
  modules.someOtherModule.services.foo();
}
```
