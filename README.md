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

