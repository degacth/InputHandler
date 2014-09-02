# InputHandler

## How to взъюзывать
Обязательно необходимо заиметь RequireJS
```
<script data-main="main" src="/bower_components/requirejs/require.js"></script>
```

Далее клиентский код грузит InputHandler.js и создаёт экземпляр свежезагруженного класса, после чего начинает слушать 
соответствующие события
```
require [
    'InputHandler.js'
], (InputHandler) ->
    element = document.getElementById 'element'
    input = new InputHandler element
```
```
    input.on 'down', (e) -> console.log e
    input.on 'up', (e) -> console.log e
    input.on 'move', (e) -> console.log e
```

```
git remote add origin git@github.com:degacth/InputHandler.git
git push -u origin master
```