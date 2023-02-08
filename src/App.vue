<template>
  <div class="app" :class="mode">
  <Header :mode="mode" @toggle="toggle" />
  <!-- <Content :mode="mode" /> -->
  <router-view/>
  </div>

  <!-- <nav>
    <router-link :mode="mode"  to="/">Home</router-link> |
    <router-link :mode="mode"  to="/about">About</router-link>
  </nav> -->

 
</template>

<script>
import Header from '@/components/Header.vue'
import Content from '@/components/Content.vue'


export default {
  name: 'app',
  data () {
    return {
      mode: 'light'
    }
  },
  components: {
    Header,
    Content,
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

<style lang="scss">
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
  background: #F3F3F3;
  color: #15202B;
  transition: background 0.3s ease-in-out;
}
.dark {
  background: #192734;
  color: #E8E8E8;
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
