<template>
  <div class="home">
    <div class="pic">

    <div class="title">

      <h3>Hi, my name is</h3>
      <h1>Leobardo D. Martinez-Quiroz</h1>

      <p class="para">
        I am a Jr. Frontend focused Software Developer building the Frontend of Websites. I like design and
      </p>
      <!-- <img src="../assets/logo.png" alt="Portfolio Image"> -->
    </div>
  </div>
</div>
</template>

<script>


export default {
  props: ['mode'],
  components: {
    
  }

}



</script>

<style scoped lang="scss">
* {
  font-family: 'Montserrat', sans-serif;
}

.content {
  padding: 25px;
}
.content h3 {
  font-size: 28px;
  text-transform: uppercase;
  font-weight: 300;
  margin-bottom: 25px;
}
// .image-grid {
//     display: grid;
//     grid-template-columns: repeat(3, 1fr);
//     grid-gap: 15px;
// }
// .image-grid .col img {
//     width: 100%;


  // picture background
  // z-index: -1;
  // background: url("../assets/logo.png") no-repeat center center
  // fixed;
  // background-attachment: local;
// }
// this will make the picture darker
// .dark .image-grid .col img {  
//     filter: brightness(85%);
// }
.title {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: flex-start;
  position: relative;
color: #DEE2E6;
  // border: black solid 4px;
  width: 100%;
  height: 600px;
//     padding: 20px;
//     border-radius: 10px;
// background: #6c757d;
// opacity: 60%;
// z-index: 1;
// top: 70px;
}
.title h1 {
  color: #5A189A;
  font-weight: 800;
  text-shadow:5px 5px #C77DFF;
  font-size: 60px;

  // font-family: 'Gajraj One', cursive;
// font-family: 'Handlee', cursive;
// font-family: 'Italianno', cursive;
// font-family: 'Montserrat', sans-serif;
// font-family: 'Poller One', cursive;
// font-family: 'Press Start 2P', cursive;
// font-family: 'Rubik Moonrocks', cursive;
// font-family: 'Tilt Prism', cursive;
// font-family: 'Titan One', cursive;
font-family: 'Ultra', serif;
// font-family: 'UnifrakturMaguntia', cursive;

}
.dark .title h1 {
  color: rgb(20, 240, 57);
  text-shadow:5px 5px #006400;


}
.title h3 {
color: #DEE2E6;
font-weight: 600;
// Start of the underline
display: block;
  position: relative;
  padding: 0.2em 0;

  overflow: hidden;
}
.title h3::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0.1em;
  background-color: #38B000;
  opacity: 0;
  transition: opacity 300ms, transform 300ms;
}
.title h3:hover::after,
.title h3:focus::after {
  opacity: 1;
  transform: translate3d(0, 0.2em, 0);
}
.title h3::after {
  opacity: 1;
  transform: translate3d(-100%, 0, 0);
}
.title h3:hover::after,
.title h3:focus::after {
      transform: translate3d(0, 0, 0);
    }
// End of the underline in Light mode
.dark .title h3 {
  color: #DEE2E6;
  font-weight: 600;
// Start of the underline
  display: block;
  position: relative;
  padding: 0.2em 0;

  overflow: hidden;

}
.dark .title h3::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0.1em;
  background-color: #7B2CBF;
  opacity: 0;
  transition: opacity 300ms, transform 300ms;
}
.dark .title h3:hover::after,
.dark .title h3:focus::after {
  opacity: 1;
  transform: translate3d(0, 0.2em, 0);
}
.dark .title h3::after {
  opacity: 1;
  transform: translate3d(-100%, 0, 0);
}
  .dark .title h3:hover::after,
  .dark .title h3:focus::after {
      transform: translate3d(0, 0, 0);
    }
// End of the underline
.title h1, h3, p {
  margin: 20px;
}

.para {
  // display: flex;
  // flex-direction: column;
  // justify-content: center;
  // // align-items: flex-end;
  // text-align: center;
  width: 100%;
  max-width: 600px;
  margin: 20px;
  z-index: 2;
  font-weight: 800;
  padding: 20px;
  border-radius: 10px;
background: #495057;
color: #CED4DA;
opacity: 85%;
// border: green solid 4px;


}
.dark .para {
  color: #DEE2E6;
}
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  
  // background: url("../assets/LDM3.JPG") no-repeat right;
  // background-size: 100% auto;
  // background-attachment: local;
}
.pic {
  width: 100%;
  // Height needs to be change when cell phone sizing !important
  height: 800px;  
  background: url("../assets/LDM3.JPG") no-repeat right;
  background-size: 100% auto;
  margin: 20px;
  border-radius: 5px;
}
.dark .pic {
  background: url("../assets/LDM4.JPG") no-repeat right;
  background-size: 100% auto;

  // background-attachment: local;
}
// @media screen and (max-width:1024px) {
//   .col {
//       height: 500px;
//   }
//   .title {
//       height: 500px;
//   }
  
// }

@media screen and (max-width:700px) {
  // .home {
  //     height: 300px;
  // }
  .title {
      height: 620px;
      top: 40px;
  }
  .title h1 {
    font-size: 30px;
    margin: 10px;
  }
  .title h3 {
    font-size: 20px;
    margin: 10px;

  }
  .para {
      margin: 10px;
      max-width: 480px;
  }
  
}
</style>