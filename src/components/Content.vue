<template>
  <div class="content">
    <h3>This is {{ mode }} mode</h3>
    <div class="image-grid">
        <div class="col">
            <img src="../assets/logo.png" alt="Portfolio Image">
        </div>
        <div class="col">
            <p class="para">
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem quo, laborum tempore earum quam ab! Ut nobis laboriosam illum iste sequi dicta, nesciunt voluptates. Doloremque minus odio nulla temporibus vero.
    </p>
            <img src="../assets/logo.png" alt="Portfolio Image">

        </div>
        <div class="col">
            <img src="../assets/logo.png    " alt="Portfolio Image">

        </div>
        
    </div>
    
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

.content {
    padding: 25px;
}
.content h3 {
    font-size: 28px;
    text-transform: uppercase;
    font-weight: 300;
    margin-bottom: 25px;
}
.image-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 15px;
}
.image-grid .col img {
    width: 100%;
    // picture background
    // z-index: -1;
    // background: url("../assets/logo.png") no-repeat center center
    // fixed;
    // background-attachment: local;
}
// this will make the picture darker
.dark .image-grid .col img {  
    filter: brightness(85%);
}
.para {
    width: 100%;
    max-width: 600px;
    margin: 25px auto 0px;
    z-index: 1;
}
</style>