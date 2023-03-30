## Vue Product Cart
[Using Vue from CDN](https://vuejs.org/guide/quick-start.html#using-vue-from-cdn)

Use Vue directly from a CDN via a script tag.
Add CDN using a script tag in `index.html`:
```
<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>
```

### To Run Locally
Use Live Server [(VS Code extension)](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

### VueJS Directives
- greeting
- isVisible
- isVisible2

v-model, v-show, v-cloak, v-if, v-else-if, v-else

### Events and Methods
- Greeting with input
- Toggle Box button, with a box that toggles from `isVisible` to !isVisible
  - Created a toggleBox() method, that is accessible anywhere in the Vue.js application

Event:
- Keyboard Event
`@keyup.enter`
```
<input @keyup.enter v-model="greeting" />
```
or the key code associated with any key on the keyboard. For enter that would be "13"
```
<input @keyup.13 v-model="greeting" />
```

Add greet method for this keyup event:
```
<input @keyup.enter="greet" v-model="greeting" />
```

@keyup`.enter` is a modifier, for using the enter key.

You can also target only right clicks:
```
<button @click.right="toggleBox">Toggle Box</button>
```
@click`.prevent` for prevent default

`@click.prevent.stop` You can chain as many of these modifiers as you want in Vue.js