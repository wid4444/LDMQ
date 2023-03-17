<template>

  <h1>
  <span>I’m a software engineer that</span>
  <div class="message">
    <div class="word1">designs</div>
    <div class="word2">builds</div>
    <div class="word3">deploys</div>
  </div>

</h1>


<p class="para">
        I’m a software engineer that builds, designs and deploys websites. 
        Currently, I’m focused on designing and building user-friendly products for small businesses as a Freelancer.
      </p>

</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
* {
  box-sizing: border-box;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  width: 100vw;
}
h1 {
  color: green;
  font-family: tahoma;
  font-size: 3rem;
  font-weight: 100;
  line-height: 1.5;
  text-transform: uppercase;
  white-space: nowrap;
  overflow: hidden;
  position: relative;
  width: 550px;
}

h1 span {
  font-size: 20px;
  margin-left: 40px;
}

.message {
  background-color: red;
  color: #333;
  display: block;
  font-weight: 900;
  font-size: 3rem;

  overflow: hidden;
  position: absolute;
  padding-left: 0.5rem;
  top: 0.2rem;
  left: 360px;
  animation: openclose 5s ease-in-out infinite;
}

.word1, .word2, .word3 {
  font-family: tahoma;
}

@keyframes openclose {
  0% {
    top: 0.2rem;
    width: 0;
  }
  5% {
    width: 0;
  }
  15% {
    width: 230px;
  }
  30% {
    top: 0.2rem;
    width: 230px;
  }
  33% {
    top: 0.2rem;
    width: 0;
  }
  35% {
    top: 0.2rem;
    width: 0;
  }
  38% {
    top: -4.5rem;
    
  }
  48% {
    top: -4.5rem;
    width: 190px;
  }
  62% {
    top: -4.5rem;
    width: 190px;
  }
  66% {
    top: -4.5rem;
    width: 0;
    text-indent: 0;
  }
  71% {
    top: -9rem;
    width: 0;
    text-indent: 5px;
  }
  86% {
    top: -9rem;
    width: 285px;
  }
  95% {
    top: -9rem;
    width: 285px;
  }
  98% {
    top: -9rem;
    width: 0;
    text-indent: 5px;
  }
  100% {
    top: 0;
    width: 0;
    text-indent: 0;
  }
}
</style>