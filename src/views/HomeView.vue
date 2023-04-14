<template>
  <div class="home">
    <div class="pic">

      <div class="title">
        <Hi :mode="mode" @toggle="toggle"/>

        <Name :mode="mode" @toggle="toggle"/>
      
        <Para :mode="mode" @toggle="toggle"/>
    </div>

  </div>
</div>

</template>

<script>
import Hi from '../components/Hi.vue'
import Name from '../components/Name.vue'
import Para from '../components/Para.vue'

export default {
  props: ['mode'],
  components: {
    Name,
    Hi,
    Para,
  }

}
</script>

<style scoped lang="scss">
.title {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: flex-start;
  position: relative;
  color: #DEE2E6;
  width: 100%;
  height: 600px;
  top: 200px;
}

.home {
  display: flex;
  justify-content: center;
  align-items: center;
}
.pic {
  width: 100%;
  // Height needs to be change when cell phone sizing !important
  height: 1000px;  
  background: url("../assets/home/1.png") no-repeat center center;
  background-size: 100% auto;
  margin: 20px;
  border-radius: 5px;
  margin-bottom: 200px;
}
.dark .pic {
  background: url("../assets/home/dark2.png") no-repeat center center;
  background-size: 100% auto;

  // background-attachment: local;
}

@media screen and (max-width:1200px) {
  .pic {
  width: 100%;
  // Height needs to be change when cell phone sizing !important
  height: 650px;  
  // background: url("../assets/LDM3.JPG") no-repeat right;
  background-size: 100% auto;
  margin: 20px;
  // border-radius: 5px;
}
// .para {
//     // margin-top: 20px;
//       margin: 0px 0px 60px 40px;
//       text-align: center;
//       max-width: 600px;
//       font-size: 18px;
//   }
}

@media screen and (max-width:700px) {
  .pic {
  width: 100%;
  // Height needs to be change when cell phone sizing !important
  height: 400px;  
  background: url("../assets/home/1c.png") no-repeat center center;
  background-size: 100% auto;
  margin: 20px;
  // border-radius: 5px;
}
.dark .pic {
  width: 100%;

  background: url("../assets/home/dark2c.png") no-repeat center center;
  background-size: 100% auto;
  margin: 20px;
}
  .title {
      height: 620px;
      top: 40px;
  }
  .title h1 {
    font-size: 30px;
    margin: 10px;
    padding-bottom: 20px;
  }
  
  
}


</style>