<template>
  <div class="portfolio">
    <h1>Some Things I've Built</h1>

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
.portfolio h1 {
  margin-top: 40px;
  
}
.projects {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 1000px;
  margin: 80px;
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

</style>