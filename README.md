# vuejs-semantic-ui

> Vue Semantic-UI boilerplate

## Build Setup

``` bash
# install dependencies
npm install

# build semantic-ui
npm run build-semaintic-ui

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

## Using Semantic-UI
import semantic JS and css at your app root file
```js
import '../semantic/dist/semantic.min.css';
import 'semantic';
```
Then you can use semantic ui classes as well as JS. For example:

```js
$('.ui.accordion')
  .accordion();
```

### configuring Semantic-UI

You can configure semantic themes using guides at http://semantic-ui.com/introduction/build-tools.html  
Call ```npm run build-semaintic-ui``` after you've made you configuration

## Using Sass

You can write Sass style directly at you Vue components like this:
```
<style lang="sass">
  h2 {
    border: 2px solid aquamarine;
  }
</style>
```
or 
import scss styles from your styles folder

```
<style lang="sass">
  @import "~styles/border"
</style>
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
