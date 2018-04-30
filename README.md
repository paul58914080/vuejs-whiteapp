# A VueJS whiteapp

This is an experience that I would like to share as a kata for a step by step process to set up a whiteapp for vue js through vue-cli (**still in beta at the time**)

### Step 1: Install the **`vue-cli`**

Thanks for the amazing cli tool from vue which has eased the development by scaffolding many of the repeated dev activities, we as developers do. Answer few simple questions and you have the cli generate code for you.. isnt that simple ??

> **`npm i -g @vue/cli`**   

See [CLI docs](https://github.com/vuejs/vue-cli/blob/dev/docs/cli.md) for all available commands.

### Step 2: Generate the whiteapp

After installing the cli I had few key strokes to type to generate a new project

> **`vue create <my-project>`**  

I liked the pick my preset, so I chose the following

- Typescript
- Progressive Web App (PWA) Support
- Router
- Veux
- CSS Pre-processors
- Linter / Formatter
- Unit Testing
- E2E Testing 

### Step 3: Install bootstrap 4

For styling the application over the years of experience, love and comfort I prefer using bootstrap. It is very simple to include it in your project

> **`npm install bootstrap --save`**   

Include it in your main page

```html
<style lang="scss">
@import '../node_modules/bootstrap/scss/bootstrap.scss';
</style>
```

### Step 4: Separation of concerns ( **`html, (s)css, (j)ts`** ) 

Each developer has their own point of view when it comes to having the code for view, style and logic to be in separate file or some of them prefer in the same. The default behaviour when you generate the components through the cli would be to have everything in the same file i.e. *.vue. However for developers who likes to keep them separate all you got to do is

**HelloWorld.vue**
```vue
<style src="./style.css"></style>
<template src="./template.html"></template>
<script>
...
</script>
```


### References

- https://github.com/vuejs/vue-cli/tree/dev/docs
- https://medium.com/@BjornKrols/integrating-and-customising-bootstrap-4-in-vue-js-cbc29ba7688e
- https://github.com/vuejs/vueify/issues/35#issuecomment-161436380