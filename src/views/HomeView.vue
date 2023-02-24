<template>
  <div class="content">
      <!-- <h3>This is {{ mode }} mode</h3> -->
      <div class="image-grid">
          <!-- <div class="col">
          <img src="../assets/logo.png" alt="Portfolio Image">
      </div> -->
          <div class="col">

              <div class="title">

                <h3>Hi, my name is</h3>
                <h1>Leobardo D. Martinez-Quiroz</h1>


              <p class="para">
                  I am a Jr. Software Developer Frontend focused Web Developer building the Frontend of Websites and Web Applications that leads to the success of the overall product
              </p>
              <!-- <img src="../assets/logo.png" alt="Portfolio Image"> -->
          </div>
          </div>
          <!-- <div class="col">
          <img src="../assets/logo.png    " alt="Portfolio Image">

      </div> -->

      </div>

  </div>
</template>

<script>
export default {
  props: ['mode']

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

  // font-family: 'Tilt Prism', sans-serif;
  font-family: 'Gajraj One', sans-serif;
// font-family: 'Handlee', sans-serif;
// font-family: 'Italianno', sans-serif;
// font-family: 'Montserrat', sans-serif;
}
.dark .title h1 {
  color: rgb(20, 240, 57);
  text-shadow:5px 5px #006400;


}
.title h3 {
color: #DEE2E6;
font-weight: 600;

}
.dark .title h3 {
  color: #DEE2E6;
  font-weight: 600;

}
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
.col {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  // height needs to be change when cell phone sizing
  height: 600px;
  background: url("../assets/LDM3.JPG") no-repeat right;
  background-size: 100% auto;
  // background-attachment: local;
}
.dark .col {
  background: url("../assets/LDM4.JPG") no-repeat right;
  background-size: 100% auto;

  // background-attachment: local;
}
@media screen and (max-width:1024px) {
  .col {
      height: 500px;
  }
  .title {
      height: 500px;
  }
  
}

@media screen and (max-width:700px) {
  .col {
      height: 300px;
  }
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
  }
  
}
</style>