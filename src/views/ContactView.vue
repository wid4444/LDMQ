<template>
  <div class="contact">

    <!-- <div class="container">
  <div class="row">
    <div class="col-md-12 text-center"> -->
      <!-- <h3 class="animate-charcter">Contact Me</h3> -->
      <h1>Contact Me</h1>
    <!-- </div>
  </div> -->
<!-- </div> -->

    <!-- <h1>Contact Me</h1> -->

    <div class="footer">

<div class="forma">

<form action="https://formsubmit.co/ldmartinezquiroz@gmail.com" method="POST">
  <input type="hidden" name="_captcha" value="false">
  <input type="text" name="_honey" style="display:none">
  <!-- <input type="hidden" name="_next" value="https://yourdomain.co/thanks.html"> -->

  <input type="text" name="name" id="name" placeholder="Name" required>
  <input type="email" name="email" id="email" placeholder="Email" required>
  <textarea name="message" id="message" cols="30" rows="4" placeholder="Message" required></textarea>
  <button type="submit">Send</button>
</form>

</div>

    <div class="info">

        <div class="resume">
          <a class="button" href="https://drive.google.com/file/d/1BSBXhPhBDsD6IS1Xnq2NLPhDIOb0gGDY/view?usp=share_link" target="_blank">My Resume</a>
    </div>

      <div class="icons">

    <a href="https://github.com/wid4444">
          <i class="github fa-brands fa-github fa-bounce"></i>
      </a>
    <a href="https://www.linkedin.com/in/leobardo-martinez/">
        <i class="linkedin fa-brands fa-linkedin fa-bounce"></i>
      </a>
    <!-- <a href="https://codepen.io/wid4444">
        <i class="codepen fa-brands fa-codepen fa-bounce"></i>
      </a> -->

      </div>

  </div>


</div>
  </div>
</template>

<script>

export default {
  
}
</script>

<style scoped lang="scss">
.contact {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  

}
.container {
  // margin: 40px;
}
.contact h1 {
  // margin-top: 50px;
  // margin-bottom: 50px;
  margin: 40px;
}
.footer{
  // margin: 40px;
  width: 100%;
  text-align: center;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  justify-content: space-evenly;

}
//BEGINNING OF FORM
.forma form{
  margin: 40px;
  padding: 30px;
  width: 600px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  // border: #ADB5BD solid 1px;
  border-radius: 10px;
  box-shadow: 0px 6px 20px 0px  #495057;
  background: url("../assets/lightform1.png") no-repeat center center;


}
.dark .forma form{
  
  // border: #ADB5BD solid 1px;
  border-radius: 10px;
  background: url("../assets/1.png") no-repeat center center;
  box-shadow: 0px 6px 20px 0px  #E9ECEF;

}

.forma form input, textarea {
  width: 100%;
  border: none;
border-radius: 7px;
margin: 5px;
padding: 7px;
background: transparent;
color: #00b4d8;
border-bottom: solid 0.5px #00b4d8;


}
.forma form textarea {
  background: transparent;
color: #00b4d8;
border-bottom: solid 0.5px #00b4d8;

}
.dark .forma form input {
  color: #72EFDD;
  border-bottom: solid 0.5px #00ffd5;

}
.dark .forma form textarea {
  background: transparent;
color: #72EFDD;
border-bottom: solid 0.5px #00ffd5;

}


.forma button {
  margin: 40px;
  padding: 5px 10px;
  border-radius: 10px;
  box-shadow: 0 0 4px #9bf6ff;
  border: solid 0.5px #00b4d8;
  background: #9bf6ff;
  color: #bdb2ff;
  font-weight: 400;
  font-size: 25px;
}
.dark .forma button {
  margin: 40px;
  padding: 5px 10px;
  border-radius: 10px;
  background: transparent;
color: #ADB5BD;
font-weight: 100;
  font-size: 25px;
  box-shadow: 0 0 4px #72EFDD;

}
// END OF FORM
.info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.icons {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  
}
// ul li p {
//   display: none;
// }

// ul li p:hover::after {
//   display: contents;
// }

.fa-brands {
  font-size: 50px;
  background: none;
  margin: 10px;
  width: 60px;
  height: 60px;
  --fa-animation-iteration-count: 0;

  // box-shadow: 10px 7px white;
}
.fa-brands:hover {
  // text-shadow: 20px 20px  #70E000;
  font-size: 40px;
  
   --fa-animation-duration: 1s;
   --fa-animation-iteration-count: 40;
   --fa-animation-timing: ease-in-out;


  // box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px, rgba(0, 0, 0, 0.3) 0px 30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
  // box-shadow: blue 0px 0px 0px 2px inset, rgb(255, 255, 255) 10px -10px 0px -3px, rgb(31, 193, 27) 10px -10px, rgb(255, 255, 255) 20px -20px 0px -3px, rgb(255, 217, 19) 20px -20px, rgb(255, 255, 255) 30px -30px 0px -3px, rgb(255, 156, 85) 30px -30px, rgb(255, 255, 255) 40px -40px 0px -3px, rgb(255, 85, 85) 40px -40px;
}
.github {
  color: #ADB5BD;

}
.github:hover {
  color: #E9ECEF;
text-shadow: 5px 5px 5px #5a189a;
}

.dark .github:hover {
  color: #E9ECEF;
text-shadow: 5px 5px 5px #9d4edd;
}
.linkedin {
  color: #ADB5BD;
}
.linkedin:hover {
color: #E9ECEF;
text-shadow: 5px 5px 5px  blue;

}
.dark .linkedin:hover {
color: #E9ECEF;
text-shadow: 5px 5px 5px  #00b4d8;

}
.codepen {
  color: #ADB5BD;
}
.codepen:hover {
color: #E9ECEF;
text-shadow: 5px 5px 5px green;

}
.resume {
  margin: 40px;
}
// resume button
.button {
  padding: 10px 20px;
  border: none;
  outline: none;
  color: #212529;
  font-weight: 600;
  background: #E9ECEF;
  cursor: pointer;
  position: relative;
  z-index: 0;
  border-radius: 10px;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  text-decoration: none;

  
}
.dark .button {
  padding: 10px 20px;
  border: none;
  outline: none;
  color: #DEE2E6;
  background: #212529;
  cursor: pointer;
  position: relative;
  z-index: 0;
  border-radius: 10px;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  text-decoration: none;
  // margin: 20px;
}

.button:before {
  content: "";
  background: linear-gradient(
    45deg,
    #ff0000,
    #ff7300,
    #fffb00,
    #48ff00,
    #00ffd5,
    #002bff,
    #7a00ff,
    #ff00c8,
    #ff0000
  );
  position: absolute;
  top: -2px;
  left: -2px;
  background-size: 400%;
  z-index: -1;
  filter: blur(5px);
  -webkit-filter: blur(5px);
  width: calc(100% + 4px);
  height: calc(100% + 4px);
  animation: glowing-button 20s linear infinite;
  transition: opacity 0.3s ease-in-out;
  border-radius: 10px;
}

@keyframes glowing-button {
  0% {
    background-position: 0 0;
  }
  50% {
    background-position: 400% 0;
  }
  100% {
    background-position: 0 0;
  }
}

.button:after {
  z-index: -1;
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  background: #222;
  left: 0;
  top: 0;
  border-radius: 10px;
}
@media screen and (max-width:1200px) {
  .footer{
  margin: 20px;
  width: 80%;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  justify-content: space-evenly;

}
}
@media screen and (max-width:700px) {

  .contact h1 {
  margin: 60px 0 0 0;
  // margin-bottom: 20px;
}
  .footer{
    margin: 60px 0 0 0;
  width: 80%;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  justify-content: space-evenly;

}
.forma form{
  margin-bottom: 40px;
  padding: 20px;
  width: 400px;
  // text-align: center;
  // display: flex;
  // flex-direction: column;
  // align-items: center;
  // justify-content: center;
  // border: #ADB5BD solid 1px;
  border-radius: 10px;
  box-shadow: 0px 6px 20px 0px  #495057;

}
.fa-brands {
  // font-size: 50px;
  // background: none;
  margin-bottom: 50px;
  // width: 60px;
  // height: 60px;
  // box-shadow: 10px 7px white;
}
}




// .animate-charcter
// {
//   //  text-transform: uppercase;
//   background-image: linear-gradient(
//     -225deg,
//     #4cc9f0 0%,
//     #3f37c9 29%,
//     #560bad 67%,
//     #f72585 100%
//   );
//   background-size: auto auto;
//   background-clip: border-box;
//   background-size: 200% auto;
//   color: #fff;
//   background-clip: text;
//   text-fill-color: transparent;
//   -webkit-background-clip: text;
//   -webkit-text-fill-color: transparent;
//   animation: textclip 2s linear infinite;
//   display: inline-block;
//       font-size: 50px;
// }

// @keyframes textclip {
//   to {
//     background-position: 200% center;
//   }
// }
</style>