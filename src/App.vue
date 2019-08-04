<template>
  <div id="app">
    <div id="nav">
      <router-link class="nav-button" to="/">Home</router-link>
      <router-link class="nav-button" to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css?family=Montserrat:300,400,600,700&display=swap");
@import url("https://fonts.googleapis.com/css?family=Merriweather:300,400,700&display=swap");

html,
body {
  background-color: #00b787;
  height: 100%;
  margin: 0;
  justify-content: space-around;
}
#app {
  display: flex;
  flex-direction: column;
  height: 100%;
  text-align: center;
  color: white;
}
#nav {
  min-height: 5%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  text-align: center;
  min-height: 10vh;
}
.nav-button {
  padding: 2% 5% 0 5%;
  color: white;
  text-decoration: none;
  font-size: xx-large;
}

.router-link-exact-active {
  background-color: blue;
  display: none;
}
</style>
