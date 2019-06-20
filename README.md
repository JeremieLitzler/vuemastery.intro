# Notes from Vue Mastery Introduction course

## Course

https://www.vuemastery.com/courses/intro-to-vue-js

## Notes

### Binding

Short hand of `v-bind` => `:` 

Ex: `v-bind:title="A title"` is the same to `:title="A title"`

Short hand of `v-on` => `@`

Ex: `v-on:mouseover="updateProductImage"` is the same as `@mouseover="updateProductImage"`

The `v-bind:style` directive can be written in two ways:

`:style="{ backgroundColor: variant.variantColor }"`
or
`:style="{ 'background-color': variant.variantColor }"`

### Computed properties

**They are cache until their dependencies change**.

### Components

- The template must contain one root element !

**OK**

```js
  `
  <div>
    <p>Some text</p>
  </div>
  `
```

**KO**

```js
  `
  <div>
    <p>Some text</p>
  </div>
  <div>
    <p>Some text</p>
  </div>
  `
```

- The `data` of a component must be a function.
- To pass on from the Vue root object to a component, you must specify the `props`.
  - **Recommandation:** define the specification of the each prop object.
  
  ```js
  props: {
    premium: {
      type: Boolean,
      required: true
    }
  }
  ```
  
  ### Events
  
  - You must name the event in kebad case: `my-event` (see [doc](https://fr.vuejs.org/v2/guide/components-custom-events.html)).
