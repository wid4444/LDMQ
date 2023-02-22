
<template>
  <div class="about">
    <h1>This is an about page</h1>
    <!-- <div class="icons"> -->
    <img class="icon" src="../assets/icons/github.svg.png" alt="">
    <img class="icon" src="../assets/icons/github1.png" alt="">
    <img class="icon" src="../assets/icons/github.png" alt="">
    <img class="icon" src="../assets/icons/github2.png" alt="">
    <img class="icon" src="../assets/icons/github3.png" alt="">
<br>
    <img class="icon" src="../assets/icons/linkedin.png" alt="">
    <img class="icon" src="../assets/icons/linkedin2.png" alt="">
    <img class="icon" src="../assets/icons/linkedin0.png" alt="">
    <img class="icon" src="../assets/icons/linkedin3.png" alt="">
    <img class="icon" src="../assets/icons/linkedin1.png" alt="">
    <img class="icon" src="../assets/icons/linkedin4.webp" alt="">

<br>
    <img class="icon" src="../assets/icons/gitlab0.png" alt="">
    <img class="icon" src="../assets/icons/gitlab.png" alt="">
    <img class="icon" src="../assets/icons/gitlab2.png" alt="">
    <img class="icon" src="../assets/icons/gitlab1.png" alt="">

<br>
    

    <img class="icon" src="../assets/icons/IntelliJ.png" alt="">
    <img class="icon" src="../assets/icons/IntelliJ1.png" alt="">
<br>
    <img class="icon" src="../assets/icons/PyCharm.png" alt="">
    <img class="icon" src="../assets/icons/PyCharm1.png" alt="">
    <img class="icon" src="../assets/icons/PyCharm.webp" alt="">

<br>
    <img class="icon" src="../assets/icons/VSCode.png" alt="">
    <img class="icon" src="../assets/icons/xcode.png" alt="">
    <img class="icon" src="../assets/icons/Replit.png" alt="">


<br>
    <img class="icon" src="../assets/icons/css1.png" alt="">
    <img class="icon" src="../assets/icons/html1.png" alt="">
    <img class="icon" src="../assets/icons/JS0.png" alt="">
    <img class="icon" src="../assets/icons/react.webp" alt="">
    <img class="icon" src="../assets/icons/react1.webp" alt="">

    <img class="icon" src="../assets/icons/Java1.png" alt="">
    <img class="icon" src="../assets/icons/java.png" alt="">

    <img class="icon" src="../assets/icons/vuejs.png" alt="">
    <img class="icon" src="../assets/icons/node.png" alt="">

    <img class="icon" src="../assets/icons/python.png" alt="">
    <img class="icon" src="../assets/icons/Python2.png" alt="">

    <img class="icon" src="../assets/icons/swiftUI.png" alt="">

    <!-- <img class="icon" src="../assets/icons/js.png" alt=""> -->
    <img class="icon" src="../assets/icons/PostgreSQL.png" alt="">
    <!-- <img class="icon" src="../assets/icons/PostgreSQL.svg" alt=""> -->
    
    
    <img class="icon" src="../assets/icons/springboot.png" alt="">
    <br>
    <img class="icon" src="../assets/icons/sass.png" alt="">
    <img class="icon" src="../assets/icons/sass1.png" alt="">

    <img class="icon" src="../assets/icons/vite.svg" alt="">
    <img class="icon" src="../assets/icons/3d-bootstrap-programming-framework-logo-free-png.webp" alt="">

    <img class="icon" src="../assets/icons/wings.gif" alt="">



    <div :class="{ shake: disabled }">
  <!-- <button @click="warnDisabled">Click me</button> -->
  <img @click="warnDisabled" class="icon" src="../assets/icons/wings.gif" alt="">
  <span v-if="disabled">This feature is disabled!</span>
</div>



  <!-- </div> -->






    


<togglertest/>

  </div>
</template>

<script>

import togglertest from '../components/togglertest.vue'
export default {
  components: {
    togglertest,
  },

  data() {
    return {
      disabled: false
    }
  },
  methods: {
    warnDisabled() {
      this.disabled = true
      setTimeout(() => {
        this.disabled = false
      }, 1500)
    }
  }

}
</script>

<style>
.icon {
  width: 150px;
  /* height: 200px; */
  border: 1px black solid;
  margin: 5px;
  border-radius: 5px;

  filter: brightness(85%);
  
}


.dark .icon {
  border: 1px white solid;
  filter: brightness(100%);
}

.shake {
  animation: shake 0.82s cubic-bezier(0.36, 0.07, 0.19, 0.97) both;
  transform: translate3d(0, 0, 0);
}

@keyframes shake {
  10%,
  90% {
    transform: translate3d(-1px, 0, 0);
  }

  20%,
  80% {
    transform: translate3d(2px, 0, 0);
  }

  30%,
  50%,
  70% {
    transform: translate3d(-4px, 0, 0);
  }

  40%,
  60% {
    transform: translate3d(4px, 0, 0);
  }
}

</style>
