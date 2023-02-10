<template>
    <div class="content">
        <!-- <h3>This is {{ mode }} mode</h3> -->
        <div class="image-grid">
            <!-- <div class="col">
            <img src="../assets/logo.png" alt="Portfolio Image">
        </div> -->
            <div class="col">

                <div class="des">
                <p class="para">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem quo, laborum tempore earum quam
                    ab! Ut nobis laboriosam illum iste sequi dicta, nesciunt voluptates. Doloremque minus odio nulla
                    temporibus vero.
                </p>
                <!-- <img src="../assets/logo.png" alt="Portfolio Image"> -->
            </div>
            </div>
            <!-- <div class="col">
            <img src="../assets/logo.png    " alt="Portfolio Image">

        </div> -->

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
// .image-grid {
//     display: grid;
//     grid-template-columns: repeat(3, 1fr);
//     grid-gap: 15px;
// }
// .image-grid .col img {
//     width: 100%;


    // picture background
    // z-index: -1;
    // background: url("../assets/logo.png") no-repeat center center
    // fixed;
    // background-attachment: local;
// }
// this will make the picture darker
// .dark .image-grid .col img {  
//     filter: brightness(85%);
// }
.des {
    display: flex;
    justify-content: flex-start;
    align-items: flex-end;
    position: relative;

    // border: black solid 4px;
    width: 100%;
    height: 600px;
//     padding: 20px;
//     border-radius: 10px;
// background: #6c757d;
// opacity: 60%;
// z-index: 1;
}

.para {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: flex-end;
    text-align: center;
    width: 100%;
    max-width: 600px;
    margin: 20px;
    z-index: 2;
    font-weight: 800;
    padding: 20px;
    border-radius: 10px;
background: #495057;
color: #161616;
opacity: 85%;
// border: green solid 4px;


}
.dark .para {
    color: #ADB5BD;
}
.col {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    // height needs to be change when cell phone sizing
    height: 600px;
    background: url("../assets/LDM3.JPG") no-repeat right;
    background-size: 100% auto;
    // background-attachment: local;
}
.dark .col {
    background: url("../assets/LDM4.JPG") no-repeat right;
    background-size: 100% auto;

    // background-attachment: local;
}
@media screen and (max-width:1024px) {
    .col {
        height: 500px;
    }
    .des {
        height: 500px;
    }
    
}

@media screen and (max-width:700px) {
    .col {
        height: 300px;
    }
    .des {
        height: 620px;
    }
    .para {
        margin: 0;
    }
    
}
</style>