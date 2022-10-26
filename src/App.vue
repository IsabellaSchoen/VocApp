<template>
  <div>
    <div v-for="navbar in navbars" :key="navbar.id">
      <router-link :to="navbar.router">{{ navbar.names }}</router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
export default {
  name: "App",
  data: function () {
    return {
      navbars: [
      { names: "Home", router:"/" },
      { names: "Einstellungen", router:"/einstellungen"}
      ]
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
nav {
  padding: 30px;
}
nav a {
  font-weight: bold;
  color: #2c3e50;
}
nav a.router-link-exact-active {
  color: #42b983;
}
</style>
