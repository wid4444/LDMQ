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
    background: #AD00D8;
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
    background: #43E8ED;
    -webkit-transition: .4s;
    transition: .4s;
}
.dark .toggler:before {
    // background: #80FFDB;
    background: rgb(222,170,255);
// background: radial-gradient(circle,  #c0fdff 0%, #4D194D 50%);

}

input:checked + .toggler {
    background: #72EFDD;

    // border: solid 0.2px #80FFDB;
}
input:focus + .toggler {
    box-shadow: 0 0 8px #80FFDB;
}
input:focus + .dark .toggler {
    box-shadow: 0 0 8px #386641;
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