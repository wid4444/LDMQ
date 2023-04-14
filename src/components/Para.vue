<template>

<h4 class="wordCarousel">
    <span>I’m a software engineer that enjoys </span>
    <div>
        <!-- Use classes 2,3,4, or 5 to match the number of words -->
        <ul class="flip5">
            <li>websites</li>
            <li>deploying</li>
            <li>and</li>
            <li>building</li>
            <li>designing</li>
        </ul>
    </div>
</h4>


<!-- <p class="para">
        I’m a software engineer that builds, designs and deploys websites. 
        Currently, I’m focused on designing and building user-friendly products for small businesses as a Freelancer.
      </p> -->

</template>

<script>
export default {
    props: ['mode']

}
</script>

<style scoped lang="scss">
.wordCarousel {
    font-size: 36px;
    font-weight: 100;
    color: #72CE27;
    margin: 0 0px 300px 70px;
    div {
        overflow: hidden;
        position: relative;
        float: right;
        height: 55px;
        padding-top: 0px;
        margin-top: 0px;
         li {
            font-family: 'Montserrat', sans-serif;
            text-transform: uppercase;
            color: #FDD54F;
    text-shadow: 0 0 6px #FDD54F;
            font-weight: 700;
            padding: 0 10px;
            height: 45px;
            margin-bottom: 45px;
            display: block;
        }
    //     li {
    //         color: #FF9900;
    // text-shadow: 0 0 6px #FF9900;
    //     } 
    }
}


.dark .wordCarousel {
    color: #ADB5BD;
}
.dark .wordCarousel div li {
    text-shadow: 0 0 6px #80ffdb;
            color: #80ffdb;
    


}

.flip2 { animation: flip2 6s cubic-bezier(0.23, 1, 0.32, 1.2) infinite; }
.flip3 { animation: flip3 8s cubic-bezier(0.23, 1, 0.32, 1.2) infinite; }
.flip4 { animation: flip4 10s cubic-bezier(0.23, 1, 0.32, 1.2) infinite; }
.flip5 { animation: flip5 12s cubic-bezier(0.23, 1, 0.32, 1.2) infinite; }

@keyframes flip2 {
    0% { margin-top: -180px; }
    5% { margin-top: -90px;  }
    50% { margin-top: -90px; }
    55% { margin-top: 0px; }
    99.99% { margin-top: 0px; }
    100% { margin-top: -180px; }
}

@keyframes flip3 {
    0% { margin-top: -270px; }
    5% { margin-top: -180px; }
    33% { margin-top: -180px; }
    38% { margin-top: -90px; }
    66% { margin-top: -90px; }
    71% { margin-top: 0px; }
    99.99% { margin-top: 0px; }
    100% { margin-top: -270px; }
}

@keyframes flip4 {
    0% { margin-top: -360px; }
    5% { margin-top: -270px; }
    25% { margin-top: -270px; }
    30% { margin-top: -180px; }
    50% { margin-top: -180px; }
    55% { margin-top: -90px; }
    75% { margin-top: -90px; }
    80% { margin-top: 0px; }
    99.99% { margin-top: 0px; }
    100% { margin-top: -360px; }
}

@keyframes flip5 {
    0% { margin-top: -450px; }
    5% { margin-top: -360px; }
    20% { margin-top: -360px; }
    25% { margin-top: -270px; }
    40% { margin-top: -270px; }
    45% { margin-top: -180px; }
    60% { margin-top: -180px; }
    65% { margin-top: -90px; }
    80% { margin-top: -90px; }
    85% { margin-top: 0px; }
    99.99% { margin-top: 0px; }
    100% { margin-top: -450px; }
}

// Layout //////////////////////////////////////////

@import url(https://fonts.googleapis.com/css?family=Roboto+Condensed:300|Oswald);
body,
html {
    width: 100%;
    height: 100vh;
    margin: 0;
    padding: 0;
    overflow: hidden;
}

body {
    // font-family: "Roboto Condensed", cursive;
    display: flex;
    align-items: center;
    justify-content: center;
    background: darkorange; 
    &::after {
        content:"";
        display: block;
        width: 110%;
        height: 125vh;
        background: radial-gradient(#222, #000);
        position: absolute;
        z-index: -1;
        transform: rotate(20deg);
        border-radius: 50%;
    }
}
@media screen and (max-width:1200px) { 
.wordCarousel {
    font-size: 28px;
    // margin: 0 0px 130px 40px;

} 

      

    }
 @media screen and (max-width:700px) {
     .wordCarousel {
    font-size: 16px;
    font-weight: 600;
    margin: 0 0px 110px 0px;
    display: flex;
    justify-content: center;
    align-items: center;
flex-wrap: wrap;
    }
    li {
            // font-family: 'Montserrat', sans-serif;
            // text-transform: uppercase;
            // text-shadow: 0 0 8px #80ffdb;
            // color: #80ffdb;
            // font-weight: 700;
            padding: 0 10px;
            // height: 45px;
            margin-bottom: 75px;
            // display: block;
        }
 }
 .dark .wordCarousel {
    color: #72CE27;
 }
</style>