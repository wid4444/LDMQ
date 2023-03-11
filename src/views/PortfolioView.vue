<template>
  <div class="portfolio">
    <h1>Some Things I've Built</h1>

    <div class="avi">
      <a href="https://www.avi-it.org/">
        <img id="logo" src="../assets/my-work/logo.jpg" alt="">
      </a>
      <h4>Responsive Vue Website for a Non-profit Organization</h4>
        <img id="avi" src="../assets/my-work/avi-it.png" alt="">
      
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
.portfolio h1 {
  margin-top: 40px;
}
.avi {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  // border: blue solid 3px;
  margin: 20px;
  // width: 100%;

}
#logo {
  width: 100px;
  border-radius: 10px;
  margin-top: 40px;
  margin-bottom: 40px;

  top: 100px;
}
#avi {
  margin-top: 40px;

  width: 800px;
  height: auto;
}
@media screen and (max-width:700px) {
  .avi h4 {
    font-size: 18px;
    text-align: center;
  }
  #logo {
  width: 80px;
}
#logo:hover {
  // width: 100px;
  box-shadow: -10px 10px 10px #b100e8;
}

  #avi {
  width: 400px;
  height: auto;
}
}

</style>