<template>
  <div class="portfolio">

    <h1 data-heading="I">Some Things I've Built</h1>

    <!-- <h1>Some Things I've Built</h1> -->

    <div class="projects">

    <div class="project">
      <a href="https://www.avi-it.org/">
        <img id="avi-logo" src="../assets/my-work/logo.jpg" alt="">
      </a>
      <h4>Responsive Vue Website for a Non-profit Organization</h4>
        <img id="mock-up" src="../assets/my-work/avi.png" alt="">
      
    </div>
<div class="project">
      <a href="https://www.avi-it.org/">
        <img id="lopez-logo" src="../assets/my-work/Lopez.png" alt="">
        <!-- <img id="lopez-logo" src="../assets/my-work/Lopez2.png" alt=""> -->
      </a>
      <h4>Responsive Vue Website for a General Contractors Company</h4>
        <img id="mock-up" src="../assets/my-work/avi-it.png" alt="">
      
    </div>


  </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
.portfolio {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  
}
// .portfolio h1 {
//   margin-top: 40px;
  
// }
.projects {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 1000px;
  margin: 120px 80px 80px 80px;
  top: 60%;
  padding: 40px;
border-radius: 20px;
box-shadow: 0px 6px 20px 0px  #495057;
background: linear-gradient(0deg, rgba(108,117,125,1) 0%, rgba(233,236,239,1) 100%);
// background: url("../assets/modern-painting.jpeg") no-repeat center center;



}
.dark .projects {
  box-shadow: 0px 6px 20px 0px  #E9ECEF;
// background: linear-gradient(0deg, rgba(33,37,41,1) 0%, rgba(206,212,218,1) 100%);
// background: linear-gradient(0deg, rgba(33,37,41,1) 0%, rgba(108,117,125,1) 100%);
// background: linear-gradient(0deg, rgba(33,37,41,1) 0%, rgba(173,181,189,1) 100%);
// background: url("../assets/neon.png") no-repeat center center;




}

.project {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  // border: blue solid 3px;
  margin: 20px;
  
  width: 100%;

}

#avi-logo {

  width: 100px;
  border-radius: 10px;
  margin-top: 40px;
  margin-bottom: 40px;

  top: 100px;
}

// #lopez1-logo {
// display: none;
// }
// .dark #lopez1-logo {
//   display: contents;

//   width: 200px;
//   border-radius: 10px;
//   margin-top: 40px;
//   margin-bottom: 40px;

//   top: 100px;
// }

// .dark #lopez-logo {
//   display: none;

// }
 #lopez-logo {
  // display: contents;
  
  width: 200px;
  border-radius: 10px;
  margin-top: 40px;
  margin-bottom: 40px;

  top: 100px;
}
#mock-up {
  margin-top: 40px;

  width: 800px;
  height: auto;
}
@media screen and (max-width:1200px) {
  .projects {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 800px;
  margin: 20px;
  padding: 20px;
border-radius: 20px;
box-shadow: 0px 6px 20px 0px  #495057;


}
#mock-up {
  width: 600px;
  height: auto;
}
}
@media screen and (max-width:700px) {
  .projects {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 500px;
  margin: 20px;
  padding: 20px;
border-radius: 20px;
box-shadow: 0px 6px 20px 0px  #495057;


}
   h4 {
    font-size: 18px;
    text-align: center;
  }
  #avi-logo {
  width: 80px;
}
#avi-logo:hover {
  // width: 100px;
  box-shadow: -10px 10px 10px #b100e8;
}
#lopez-logo {
  width: 100px;
}

  #mock-up {
  width: 450px;
  height: auto;
}
}





$h1:  #ADB5BD;
$blue: #98b5cc;
$yellow: #bc00dd;
$outline: rgba(#ADB5BD, .4);
// $shadow: rgba($yellow, .2);
// html,
// body {
//   background: linear-gradient(45deg, rgba(45,45,45,1) 9%,rgba(0,0,0,1) 100%);
//   width: 100%;
//   height: 100%;
// }

h1 {
  font-family: 'Montserrat', sans-serif;

  font-size: 40px;
  text-align: center;
  line-height: 1;
  margin: 20px;
  top: 15%;
  left: 50%;
  transform: translate(-50%, -50%);
  position: absolute;
  color: $h1;
  letter-spacing: 2px;
  
  &:before {
    content: attr(data-heading);
    position: absolute;
    overflow: hidden;
    color: $yellow;
    width: 100%;
    z-index: 5;
    text-shadow: none;
    left: 60.5%;
    text-align: left;
    animation: flicker 3s linear infinite;
  }
}

@keyframes flicker {
  0%, 19.999%, 22%, 62.999%, 64%, 64.999%, 70%, 100% {
    opacity: .99;
    text-shadow: -1px -1px 0 $outline, 1px -1px 0 $outline, -1px 1px 0 $outline, 1px 1px 0 $outline, 0 -2px 8px, 0 0 2px, 0 0 2px #9900ff, 0 0 4px #d744ff, 0 0 2px #9900ff, 0 2px 3px #000;
  }
  20%, 21.999%, 63%, 63.999%, 65%, 69.999% {
    opacity: 0.4;
    text-shadow: none;
  }
}

/*
 * Webfont: CoreCircus by S-Core
 * URL: http://www.myfonts.com/fonts/s-core/core-circus/regular/
 * Copyright: Copyright (c) 2013 by S-Core Co., Ltd.. All rights reserved.
 * Licensed pageviews: 10,000
*
 * Webfont: CoreCircus2DDot1 by S-Core
 * URL: http://www.myfonts.com/fonts/s-core/core-circus/dot1/
 * Copyright: Copyright (c) 2013 by S-Core Co., Ltd.. All rights reserved.
 * Licensed pageviews: 10,000
*/

@font-face {
  font-family: 'CoreCircus2DDot1';
  src: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_1_0.eot');
  src: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_1_0.eot?#iefix') format('embedded-opentype'), url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_1_0.woff2') format('woff2'), url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_1_0.woff') format('woff'), url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_1_0.ttf') format('truetype');
}

@font-face {
  font-family: 'CoreCircus';
  src: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_8_0.eot');
  src: url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_8_0.eot?#iefix') format('embedded-opentype'), url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_8_0.woff2') format('woff2'), url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_8_0.woff') format('woff'), url('https://s3-us-west-2.amazonaws.com/s.cdpn.io/209981/333BF4_8_0.ttf') format('truetype');
}
</style>