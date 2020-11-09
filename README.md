# ajcwebdev-create-nuxt-app

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).

# Mintbean - Yarn

## Create Nuxt App

```bash
yarn create nuxt-app ajcwebdev-create-nuxt-app
```

## Setup Questions

```
? Project name: (ajcwebdev-create-nuxt-app)
? Programming language: JavaScript
? Package manager: Yarn
? UI framework: None
? Nuxt.js modules: None
? Linting tools: None
? Testing framework: None
? Rendering mode: Universal (SSR / SSG)
? Deployment target: Static (Static/JAMStack hosting)
? Development tools: None
? What is your GitHub username?: ajcwebdev
? Version control system: Git
```

## Navigate into project and start dev server

```bash
cd ajcwebdev-create-nuxt-app
code .
yarn dev
```

# Mintbean - NPM

## Create Nuxt App

```bash
npx create-nuxt-app ajcwebdev-create-nuxt-app
```

## Setup Questions

```
? Project name: (ajcwebdev-create-nuxt-app)
? Programming language: JavaScript
? Package manager: Npm
? UI framework: None
? Nuxt.js modules: None
? Linting tools: None
? Testing framework: None
? Rendering mode: Universal (SSR / SSG)
? Deployment target: Static (Static/JAMStack hosting)
? Development tools: None
? What is your GitHub username?: ajcwebdev
? Version control system: Git
```

## Navigate into project and start dev server

```bash
cd ajcwebdev-create-nuxt-app
code .
npm run dev
```

## Commit to GitHub

```bash
git add .
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/ajcwebdev/ajcwebdev-create-nuxt-app.git
git remote -v
git push -u origin main
```

## Delete the following
* `assets`
* `middleware`
* `plugins`
* `store`
* `Logo.vue` in `components` folder

## Home Page

```html
// pages/index.vue

<template>
  <div class="container">

    <div>
      <h1 class="title">ajcwebdev</h1>

      <div class="links">
        <a
          href="https://dev.to/ajcwebdev"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Blog
        </a>
        <a
          href="https://github.com/ajcwebdev"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>

    </div>

  </div>
</template>
```

## About Page

```html
// pages/about.vue

<template>
  <div class="container">

    <div>
      <h1 class="title">About</h1>
      <p>This page tells you about stuff</p>
    </div>

  </div>
</template>
```

## Navigation Bar in Layouts

```html
// layouts/default.vue

<template>
  <div>
    <ul>
      <li>
        <NuxtLink to="/">Home</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/about">About</NuxtLink>
      </li>
    </ul>

    <Nuxt />
  </div>
</template>
```

## `netlify.toml` for Deploying to Netlify

```toml
[build]
  publish = "dist/"
  command = "nuxt generate"
```

```bash
git add .
git commit -m "Wooooooo!!!"
git push origin
```
