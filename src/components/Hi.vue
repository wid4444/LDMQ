<template>
    <div class="hi">Hola! Yo soy</div>
  
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">

.hi {
color: #DEE2E6;
font-weight: 600;
 top: -180px;
 font-size: 30px;
// Start of the underline
display: block;
  position: relative;
  padding: 0.2em 0;
  margin-left: 100px;

  overflow: hidden;
}
.hi::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0.1em;
  // background: linear-gradient(-45deg, #ee04f6 10%, #04f8d7 50%, #8b10f6 90%);
  background: linear-gradient(
    45deg,
    #ff0000,
    #ff7300,
    #fffb00,
    #48ff00,
    #00ffd5,
    #002bff,
    #7a00ff,
    #ff00c8,
    #ff0000
  );
  opacity: 0;
  transition: opacity 300ms, transform 300ms;
}
.hi:hover::after,
.hi:focus::after {
  opacity: 1;
  transform: translate3d(0, 0.2em, 0);
}
.hi::after {
  opacity: 1;
  transform: translate3d(-100%, 0, 0);
}
.hi:hover::after,
.hi:focus::after {
      transform: translate3d(0, 0, 0);
    }
// End of the underline in Light mode
.dark .hi {
  color: #DEE2E6;
  font-weight: 600;
// Start of the underline
  display: block;
  position: relative;
  padding: 0.2em 0;

  overflow: hidden;

}
.dark .hi::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 0.1em;
  // background: linear-gradient(-45deg, #ee04f6 10%, #04f8d7 50%, #8b10f6 90%);
  background: linear-gradient(
    45deg,
    #ff0000,
    #ff7300,
    #fffb00,
    #48ff00,
    #00ffd5,
    #002bff,
    #7a00ff,
    #ff00c8,
    #ff0000
  );
  -webkit-animation: Animation 5s ease infinite;
    -moz-animation: Animation 5s ease infinite;
    animation: Animation 5s ease infinite;
    
  // animation: title-h3 20s linear infinite;
  // transition: opacity 0.3s ease-in-out;
  opacity: 0;
  transition: opacity 300ms, transform 300ms;
}
// @-webkit-keyframes Animation {
//     0%{background-position:10% 0%}
//     50%{background-position:91% 100%}
//     100%{background-position:10% 0%}
// }
// @-moz-keyframes Animation {
//     0%{background-position:10% 0%}
//     50%{background-position:91% 100%}
//     100%{background-position:10% 0%}
// }
@keyframes Animation { 
    0%{background-position:10% 0%}
    50%{background-position:91% 100%}
    100%{background-position:10% 0%}
}



.dark .hi:hover::after,
.dark .hi:focus::after {
  opacity: 1;
  transform: translate3d(0, 0.2em, 0);
}
.dark .hi::after {
  opacity: 1;
  transform: translate3d(-100%, 0, 0);
}
  .dark .hi:hover::after,
  .dark .hi:focus::after {
      transform: translate3d(0, 0, 0);
    }
    @media screen and (max-width:700px) {
      .hi {
// color: #DEE2E6;
// font-weight: 600;
 top: -100px;
 left: 30px;
//  font-size: 30px;
// Start of the underline
// display: block;
//   position: relative;
//   padding: 0.2em 0;
//   margin-left: 100px;

//   overflow: hidden;
}
    }
</style>