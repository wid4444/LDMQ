<template>
  <div class="contact">

    <h1>Contacte Me</h1>

    <div class="footer">

<div class="forma">

<form>
  <input type="text" name="name" id="name" placeholder="Name" required>
  <input type="email" name="email" id="email" placeholder="Email" required>
  <textarea name="message" id="message" cols="30" rows="4" placeholder="Message"></textarea>
  <button type="submit">Send</button>
</form>

</div>

    <div class="info">

      <button>Resume</button>

      <div class="icons">
        <i class="github fa-brands fa-github"></i>
        <i class="linkedin fa-brands fa-linkedin"></i>
        <i class="codepen fa-brands fa-codepen"></i>
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
.footer{
  margin: 20px;
  width: 100%;
  text-align: center;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  justify-content: space-evenly;

}
.forma form{
  margin: 20px;
  padding: 20px;
  width: 500px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

}
.forma form input, textarea {
  width: 100%;
border-radius: 7px;
margin: 5px;

}
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