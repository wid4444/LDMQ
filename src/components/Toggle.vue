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

<style lang="scss">
* {
    font-family: 'Montserrat', sans-serif;
  }
.toggle {
    position: relative;
    display: inline-block;
    width: 60px;
    height: 34px;
    padding-right: 20px;
    
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
    background: #15202B;
    -webkit-transition: .4s;
    transition: .4s;

}
.toggler:before {
    position: absolute;
    content: "";
    height: 26px;
    width: 26px;
    left: 4px;
    bottom: 4px;
    background: #FFF;
    -webkit-transition: .4s;
    transition: .4s;
    right: 10px;
}
input:checked + .toggler {
    background: linear-gradient(-45deg, #ee04f6 10%, #04f8d7 50%, #8b10f6 90%);
}
input:focus + .toggler {
    box-shadow: 0 0 2px #721ef0;
}
input:checked + .toggler:before {
    -webkit-transform: translateX(26px);
    -ms-transform: translateX(26px);
    transform: translateX(26px);
}
.toggler.round {
    border-radius: 34px;
    // right: 10px;
}
.toggler.round:before {
    border-radius: 50%;
}
</style>