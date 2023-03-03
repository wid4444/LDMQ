<template>
  <div class="contact">
    this is for contact information


    <div class="icons">
      <i class="github fa-brands fa-github"></i>
      <i class="linkedin fa-brands fa-linkedin"></i>
    <i class="codepen fa-brands fa-codepen"></i>
  </div>


  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
.icons {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}


.fa-brands {
  font-size: 100px;
  background: none;
  margin: 30px;
  // box-shadow: 10px 7px white;
}
.fa-brands:hover {
  text-shadow: 20px 20px  #70E000;
  font-size: 100px;

  // box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
  // box-shadow: blue 0px 0px 0px 2px inset, rgb(255, 255, 255) 10px -10px 0px -3px, rgb(31, 193, 27) 10px -10px, rgb(255, 255, 255) 20px -20px 0px -3px, rgb(255, 217, 19) 20px -20px, rgb(255, 255, 255) 30px -30px 0px -3px, rgb(255, 156, 85) 30px -30px, rgb(255, 255, 255) 40px -40px 0px -3px, rgb(255, 85, 85) 40px -40px;
}
.github {
  color: #5A189A;
}
.github:hover {
color: #E9ECEF;
text-shadow: -10px 10px #9D4EDD;


}
.linkedin {
  color: blue;
}
.linkedin:hover {
color: #E9ECEF;
text-shadow: 0px 10px  blue;

}.codepen {
  color: green;
}
.codepen:hover {
color: #E9ECEF;
text-shadow: 10px 10px green;

}
</style>