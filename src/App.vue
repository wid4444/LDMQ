<template>
  <div class="app" :class="mode">

    <Header :mode="mode" @toggle="toggle" />

    <!-- <Hamburger class="hamburger" :mode="mode" @toggle="toggle" /> -->

    <router-view />

  </div>


</template>

<script>
import Header from './components/Header.vue'
import Hamburger from './components/Hamburger.vue'


export default {
  name: 'app',
  data () {
    return {
      mode: 'light'
    }
  },
  components: {
    Header,
    Hamburger,
  },

  created () {
    window.addEventListener('keyup', this.keyPress)
  },

  methods: {
    keyPress (e) {
      if (e.key === 'd') {
        this.toggle()
      }
    },

    toggle () {
      if (this.mode === "dark") {
        this.mode = "light"
      } else {
        this.mode = "dark"
      }
    }

  }
}
</script>

<style scoped lang="scss">
// .hamburger {
// display: none;
// }
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
  
}
.app {
  width: 100vw;
  min-height: 100vh;
  margin: 5px;
  background: #F8F9FA;
  color: #495057;
  transition: background 0.3s ease-in-out;
}
.dark {
  background: #272640;
  color: #DEE2E6;
}
// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
// }

// nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
</style>
