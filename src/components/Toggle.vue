<template>

  <div class="toggle-wrapper">

    <label class="toggle">
        <input 
        type="checkbox" 
        :checked="(mode === 'dark') ? 'checked' : false"
        @change="$emit('toggle')"
        />
        <span class="toggler round"></span>
    </label>

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
.toggle {
    position: relative;
    display: inline-block;
    // SLIDING BUTTON This will make the sliding oval smaller
    width: 30px;
    height: 17px;
    padding-right: 10px;
    
}
.toggle input {
    opacity: 0;
    width: 0;
    height: 0;
}
.toggler {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0px;
    right: 0px;
    bottom: 0;
    background: #8f07f7;
    -webkit-transition: .4s;
    transition: .4s;

}
.toggler:before {
    position: absolute;
    content: "";
    // SLIDING BUTTON This will make the sliding button smaller
    height: 13px;
    width: 13px;
    left: 2px;
    bottom: 2px;
    right: 5px;

    background: #FFF;
    // background-image: "fa-solid fa-moon";
    -webkit-transition: .4s;
    transition: .4s;
    

}
.dark .toggler:before {
    background: rgb(0, 0, 0);
//   background: url("../assets/1821-night-sky-moon-stars-outline\ \(1\).gif") no-repeat right;

}
input:checked + .toggler {
    // background: linear-gradient(-45deg, #ee04f6 10%, #04f8d7 50%, #8b10f6 90%);
    background: rgb(20, 240, 57);
}
input:focus + .toggler {
    box-shadow: 0 0 2px #721ef0;
}
input:checked + .toggler:before {
    // SLIDING BUTTON This will change the distance the slider moves
    -webkit-transform: translateX(13px);
    -ms-transform: translateX(13px);
    transform: translateX(13px);
}
.toggler.round {
    border-radius: 34px;
    // right: 10px;
}
.toggler.round:before {
    border-radius: 50%;
}
</style>