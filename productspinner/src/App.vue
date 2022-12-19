<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/products">Products</router-link>
  </nav>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000000;
}

body {
  background: rgb(253, 255, 135);
  background: linear-gradient(90deg, rgba(253, 255, 135, 1) 27%, rgba(255, 151, 212, 1) 56%, rgba(131, 255, 218, 1) 94%);
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: rgb(0, 0, 0);
}

nav a:hover {
  font-weight: bold;
  color: rgba(131, 255, 218, 1);
}

nav a.router-link-exact-active {
  color: rgb(0, 0, 0);
}
</style>
