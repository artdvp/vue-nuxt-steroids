# Nuxt Steroids

- Allows Creation of Universal Vue Apps
- Server-side Rendering
- Builds up on Vue.js
- Configuration via File & Folder Structure

## create nuxt app 

link : [create-nuxt-app](https://github.com/nuxt-community/create-nuxt-app)

```
$ npm install -g create-nuxt-app

# create 
$ npx create-nuxt-app <my-project>
$ yarn create nuxt-app <my-project>

$ cd my-nuxt-app
$ npm run dev
```

## Built with Nuxt.js

- Universal App
    - First View is rendered dynamically on the Server
    - After first load, Application turns into SPA
    - Greate for SEO
- Single Page App
    - App starts after first load
    - App stays SPA
    - Like a normal Vue App but simplified Development
- Static App
    - Pre-rendered Views are Loaded 
    - After first load, Application turns into SPA
    - Greate for SEO

## Nuxt.js Pages, Routing & Views

### From Config To Folders & Files

real routing
```js
{
    path: '/',
    component: WelcomeComponent
},
// /
// index.vue

{
    path: '/products',
    component: ProductsComponent
},
// /products
// /products/index.vue

{
    path: '/products/:id',
    component: ProductComponent
}

// /products/_id
// /products/index.vue
```

# Handling Data & Vuex

- Load and Manage Data With Ease

## Resource & Link

- More on Flexbox : https://academind.com/learn/css/understanding-css/the-position-property
- More on Routing in Nuxt: https://nuxtjs.org/guide/routing
- More on Views, Layouts etc: https://nuxtjs.org/guide/views

