
<template>
  <div class="about">

<div class="description">
  <p class="des">

Hi! My name is Leobardo but my friends and family call me <strong>Danny.</strong>  When I was 14 years old I emigrated to the United States in search of the American Dream. 

I'm a Full Stack Java Software Developer based in Middletown, DE. I am bi-lingual and have over 10 years of experience in manufacturing. I am a self-taught artist and woodworker. I have volunteered at a nonprofit organization to paint murals around the city of Wilmington DE and collaborated with other groups on smaller projects. About three years ago I found a passion for woodworking, and since then I have created a number of projects like cabinets floating shelves, and even a small bar. With my attention to detail, creativity, and communication. I like to create responsive, and user-friendly application ideas. I am always interested in learning new languages and frameworks, improving my skills, and making a contribution to society.

  </p>
</div>

<h1>Skills</h1>

<div class="skills">

<div class="skill">
  <i class="vue fa-brands fa-vuejs"></i>
  <h5>Vue.js</h5>
</div>

<div class="skill">
  <i class="html fa-brands fa-html5"></i>
  <h5>HTML</h5>
</div>

<div class="skill">
  <i class="css fa-brands fa-css3-alt"></i>
<h5>CSS</h5>
</div>

  <div class="skill">
  <i class="js fa-brands fa-square-js"></i>
  <h5>JavaScript</h5>
</div>

  <div class="skill">
    <i class="java fa-brands fa-java"></i>
    <h5>Java</h5>
  </div>

    <div class="skill">
    <i class="sass fa-brands fa-sass"></i>
    <h5>Sass</h5>
  </div>

    <div class="skill">
    <i class="git fa-brands fa-git-alt"></i>
    <h5>Git</h5>
  </div>

    <div class="skill">
    <i class="gitlab fa-brands fa-gitlab"></i>
    <h5>Git Lab</h5>
  </div>

    <div class="skill">
    <i class="github fa-brands fa-github"></i>
    <h5>GitHub</h5>
  </div>

    <div class="skill">
    <i class="react fa-brands fa-react"></i>
    <h5>React.js</h5>
  </div>

    <div class="skill">
    <i class="swift fa-brands fa-swift"></i>
    <h5>Swift UI</h5>
  </div>
</div>

<div class="tools">
    <img class="icon" src="../assets/icons/IntelliJ.png" alt="">
    <img class="icon" src="../assets/icons/PyCharm.png" alt="">
    <img class="icon" src="../assets/icons/VSCode.png" alt="">
    <img class="icon" src="../assets/icons/xcode.png" alt="">
    <img class="icon" src="../assets/icons/PostgreSQL.png" alt="">
  </div>
    

    





  <!-- <div class="skills">
      <h2>Languages</h2>
        <img class="icon" src="../assets/icons/vuejs.png" alt="">
        <img class="icon" src="../assets/icons/css1.png" alt="">
        <img class="icon" src="../assets/icons/html1.png" alt="">
        <img class="icon" src="../assets/icons/JS0.png" alt="">
        <img class="icon" src="../assets/icons/java.png" alt="">
        <img class="icon" src="../assets/icons/react.webp" alt="">
        <img class="icon" src="../assets/icons/python.png" alt="">
        <img class="icon" src="../assets/icons/swiftUI.png" alt=""> 
      <br>
      <h2>Code Editors</h2>
        <img class="icon" src="../assets/icons/VSCode.png" alt="">
        <img class="icon" src="../assets/icons/IntelliJ.png" alt="">
        <img class="icon" src="../assets/icons/Replit.png" alt="">
        <img class="icon" src="../assets/icons/xcode.png" alt="">
        <img class="icon" src="../assets/icons/PyCharm.png" alt="">
       <br>
      <h2>Other Tools</h2>
        <img class="icon" src="../assets/icons/github3.png" alt="">
        <img class="icon" src="../assets/icons/gitlab0.png" alt="">
        <img class="icon" src="../assets/icons/PostgreSQL.png" alt="">   
        <img class="icon" src="../assets/icons/springboot.png" alt="">
        <img class="icon" src="../assets/icons/node.png" alt="">
        <img class="icon" src="../assets/icons/sass1.png" alt="">
        <img class="icon" src="../assets/icons/vite.svg" alt="">
        <img class="icon" src="../assets/icons/3d-bootstrap-programming-framework-logo-free-png.webp" alt="">

      </div> -->

    <!-- <div :class="{ shake: disabled }"> -->
  <!-- <button @click="warnDisabled">Click me</button> -->
  <!-- <img @click="warnDisabled" class="icon" src="../assets/icons/wings.gif" alt="">
  <span v-if="disabled">This feature is disabled!</span>
</div> -->

  </div>
  
</template>

<script>

export default {
  components: {
    
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

<style scoped lang="scss">
.about {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 20px;
}

.des {
  text-align: center;
  margin: 20px;
  padding: 20px 100px;
  border: solid 1px white;
  border-radius: 20px;
  width: 1200px;
  // -webkit-animation: slide-right 0.8s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
	//         animation: slide-right 0.8s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
}
.des:hover {
  color: gray;
  background: #495057;
  // box-shadow: rgba(0, 0, 0, 0.17) 0px -23px 25px 0px inset, rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset, rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
  text-align: left;
  box-shadow: rgba(0, 0, 0, 0.56) 0px 22px 70px 4px;

  
}
.dark .des:hover {
  color: gray;
  background: #CED4DA;
  // box-shadow: rgba(0, 0, 0, 0.17) 0px -23px 25px 0px inset, rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset, rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px, rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px, rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
  text-align: left;
  box-shadow: rgba(255, 254, 254, 0.6) 0px 22px 70px 4px;

  
}
.skill h5:hover {
  background: linear-gradient(-45deg, #42b883 10%, #35495e 50%, #42b883 90%);
  // background: linear-gradient(-45deg, #ee04f6 10%, #04f8d7 50%, #8b10f6 90%);

  border-radius: 15px;
  margin: 10px;
  padding: 5px 0;
}
.skills {
  text-align: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  // justify-content: space-around;
  // border: solid 1px white;

  width: 100%;
  margin: 20px;
}
.tools {
  text-align: center;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  // justify-content: space-around;
  // border: solid 1px white;

  // width: 100%;
  // margin: 20px;
}
.icon {
width: 80px;
// box-shadow: 20px 20px  #70E000;
margin: 20px;
padding: 20px;
// background: #ADB5BD;
// border-radius: 50%;
}
.icon:hover {
  width: 100px;

}
.fa-brands {
  font-size: 50px;
  // background: none;
  margin: 0 20px;
  width: 120px;
  height: 120px;
  // background: #ADB5BD;
border-radius: 50%;
text-align: center;
display: flex;
flex-direction: row;
align-items: center;
justify-content: center;
// justify-content: space-around;
  // box-shadow: 10px 7px white;
}
.fa-brands:hover {
  // text-shadow: 20px 20px  #70E000;
  font-size: 70px;

  // box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
  // box-shadow: blue 0px 0px 0px 2px inset, rgb(255, 255, 255) 10px -10px 0px -3px, rgb(31, 193, 27) 10px -10px, rgb(255, 255, 255) 20px -20px 0px -3px, rgb(255, 217, 19) 20px -20px, rgb(255, 255, 255) 30px -30px 0px -3px, rgb(255, 156, 85) 30px -30px, rgb(255, 255, 255) 40px -40px 0px -3px, rgb(255, 85, 85) 40px -40px;
}
.vue {
color: #42b883;
}
.vue:hover {
color: #35495e;
text-shadow: 10px 10px #42b883;
}
.dark .vue:hover {
color: #CED4DA;
text-shadow: 10px 10px #42b883;
}
.vue h5 {
color: #42b883;
}


.html  {
  color: #e34c26;
}
.html:hover  {
  color: #495057;
text-shadow: 10px 10px #e34c26;
}
.dark .html:hover  {
  color: #CED4DA;
text-shadow: 10px 10px #e34c26;
}
// .html h5 {
//   color: #ebebeb;
  
// }

.html h5:hover {
  color: #e34c26;
  
}


.css:hover  {
  color: #1650cc;
}
.js:hover  {
  color: #bacc16;
}
.java:hover  {
  color: #169fcc;
}
.sass:hover  {
  color: #cc16b4;
}
.git:hover  {
  color: #cc6e16;
}.gitlab:hover  {
  color: #cc4016;
}.github:hover  {
  color: #8c16cc;
}.react:hover  {
  color: #16aecc;
}
.swift:hover  {
  color: #1656cc;
}




// @-webkit-keyframes slide-right {
//   0% {
//     -webkit-transform: translateX(-500px);
//             transform: translateX(-500px);
//   }
//   100% {
//     -webkit-transform: translateX(50px);
//             transform: translateX(50px);
//   }
// }
// @keyframes slide-right {
//   0% {
//     -webkit-transform: translateX(-500px);
//             transform: translateX(-500px);
//   }
//   100% {
//     -webkit-transform: translateX(50px);
//             transform: translateX(50px);
//   }
// }
.des strong {
  color: turquoise;
  font-weight: 200;

  // display: block;
  // position: relative;
  // padding: 0.2em 0;

}
// .des strong::after {
//   opacity: 1;
//   transform: scale(0);
//   transform-origin: center;
// }

// .des strong:hover::after,
// .des strong:focus::after{
//   transform: scale(1);
// }

// .des strong {
//   overflow: hidden;
// }

// .des strong::after {
//   opacity: 1;
//   transform: translate3d(-100%, 0, 0);
// }

// .des strong:hover::after,
// .des strong:focus::after{
//   transform: translate3d(0, 0, 0);
// }








.icon {
  width: 120px;
  /* height: 200px; */
  // border: 1px black solid;
  margin: 20px;
  padding: 20px;
  // background: #ADB5BD;
  // border-radius: 15px;

  filter: brightness(85%);
  
}


.dark .icon {
  // border: 1px white solid;
  filter: brightness(100%);
}


// .shake {
//   animation: shake 0.82s cubic-bezier(0.36, 0.07, 0.19, 0.97) both;
//   transform: translate3d(0, 0, 0);
// }

// @keyframes shake {
//   10%,
//   90% {
//     transform: translate3d(-1px, 0, 0);
//   }

//   20%,
//   80% {
//     transform: translate3d(2px, 0, 0);
//   }

//   30%,
//   50%,
//   70% {
//     transform: translate3d(-4px, 0, 0);
//   }

//   40%,
//   60% {
//     transform: translate3d(4px, 0, 0);
//   }
// }

</style>
