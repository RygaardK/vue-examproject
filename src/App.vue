<template>
  <div id="app">
    <header>
      <Header />
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/contact">Contact</router-link>
    </header>
    <main>
      <router-view />
    </main>
    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Footer from "@/components/Footer.vue";
import Header from "@/components/Header.vue";
export default {
  components: {
    Footer,
    Header
  }
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
header {
  height: 20vh;
  background: #333333;
  color: white;
  padding: 1em;
}
header a {
  color: white;
}

main {
  min-height: calc(100vh  - 30vh);
  padding: 1em;
}

footer {
  height: 10vh;
  background: #333333;
  color: white;
  padding: 1em
}
</style>
