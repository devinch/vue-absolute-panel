## vue-absolute-panel

a absolute position panel and auto size 

### usage
1. install package  
```
$ npm install @devinch/vue-absolute-panel -S
```

2. import to main.js file
```
import AbsolutePanel from '@devinch/vue-absolute-panel'  
Vue.component('absolute-panel', AbsolutePanel)
```

3. type to templates
```
<absolute-panel>
	<div>custom content</div>
</abslute-panel>
```

### component props
|   name   |   type   |   default   |   description   | 
|   ----   |   ----   |   -------   |   -----------   |
|   top    |   string |   auto      |                 |
|   right  |   string |   auto      |                 |
|   bottom |   string |   auto      |                 |
|   left   |   string |   auto      |                 |
|   zIndex |   number |   9         |                 | 



