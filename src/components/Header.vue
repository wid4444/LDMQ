<template>

<div class="header">
  <div class="color">

    <h1>{{ mode }} Mode</h1>

    <div class="toggle">
      <Toggle :mode="mode" @toggle="$emit('toggle')" />
    </div>
  </div>

  <header>


    <!-- <h1>
            Leobardo D. Martinez-Quiroz
        </h1> -->

    <div class="nav-links">
      <nav>
        <router-link class="nav-link" :mode="mode" to="/">Home</router-link>
        <router-link class="nav-link" :mode="mode" to="/about">About</router-link>
        <router-link class="nav-link" :mode="mode" to="/portfolio">Portfolio</router-link>
        <router-link class="nav-link" :mode="mode" to="/contact">Contact</router-link>

        <!-- <div class="nav-link">Portfolio</div>
            <div class="nav-link">Contact</div> -->

        <!-- <HamburgerMenu :mode="mode" /> -->
      </nav>
    </div>

    <div class="dropdown">
      <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
        <i class="fa-solid fa-burger fa-bounce"></i>
        <!-- <i class="fa-solid fa-burger"></i>
        <i class="fa-solid fa-bars"></i>
        <i class="fa-solid fa-bars"></i> -->

      </button>
      <ul class="dropdown-menu">
        <li><router-link class="nav-link" :mode="mode" to="/">Home</router-link></li>
        <li><router-link class="nav-link" :mode="mode" to="/about">About</router-link></li>
        <li><router-link class="nav-link" :mode="mode" to="/portfolio">Portfolio</router-link></li>
        <li><router-link class="nav-link" :mode="mode" to="/contact">Contact</router-link></li>

      </ul>
    </div>



  </header>
</div>
</template>


<script>
// @ is an alias to /src
import Toggle from './Toggle.vue'
// import HamburgerMenu from './HamburgerMenu.vue'


export default {
props: ['mode'],
components: {
  Toggle,
//   HamburgerMenu,

  
}
}
</script>



<style scoped lang="scss">

.fa-burger {
  //  --fa-animation-duration: 3s;
   --fa-animation-iteration-count: 0;
  //  --fa-animation-timing: ease-in-out;
}
.fa-burger:hover {
   --fa-animation-duration: 1s;
   --fa-animation-iteration-count: 20;
   --fa-animation-timing: ease-in-out;
}
.dropdown-toggle {
  background: #F8049C;
}
.dropdown-toggle:hover {
  background: #95E214;
}

.dark .dropdown-toggle {
  background: #272640;
  // background: url("../assets/neon.png") no-repeat center center;

}

.dark .dropdown-toggle:hover {
  background: #312244;
}
.btn {
  color: #FDD54F;
}
.dark .btn {
  color: #80FFDB;
}

.fa-burger {
  color: #FDD54F;
  font-size: 35px;
  text-shadow: 0px 0px 4px #F8049C;
  // font-family: 'Open Sans', sans-serif;

  // filter:drop-shadow(20px 10px 1px red)

  // text-shadow: 1px 6px rgba(255,0,0,.5)

// box-shadow:0 .5rem 1rem 0 rgb(224, 170, 255),0 .375rem 1.25rem 0 rgb(199, 125, 255)
}
.dark .fa-burger {
  color: #9d4edd;
  text-shadow: 0px 0px 8px  #72efdd;

  // color: rgb(20, 240, 57);
  // background: url("../assets/neon.png") no-repeat center center;

  // text-shadow: none;
}

.dropdown {
  display: none;
}
.color {
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    align-items: center;
    margin: 0px 20px;
    padding: 10px;
}
// .toggle {
//   // margin-right: 40px;
  
// }

* {
  // font-family: 'Montserrat', sans-serif;
  margin: 0;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 25px;
  margin: 0px 20px;
  height: 60px;
  border-radius: 5px;
  // background: #CED4DA;
  transition: background 0.3s ease-in-out;
}
.dark header {
  // background: #343A40;
}
// header h1 {
//   display: flex;
//   justify-content: center;
//   align-items: center;
//   font-size: 35px;
//   // text-transform: uppercase;
//   font-weight: 600;
//   // margin-left: 0px;
//   margin: 0;
//   color: #9D4EDD;
//   // font-family: 'Gajraj One', sans-serif;
// font-family: 'Handlee', sans-serif;
// // font-family: 'Italianno', sans-serif;
// // font-family: 'Montserrat', sans-serif;

// }
// .dark header h1 {
// color: #70E000;
// }
.color h1 {
    margin-right: 10px;
  text-transform: uppercase;
  font-size: 18px;
  margin-bottom: 0;

}
header nav {
  display: flex;
  height: 50px;
  margin-left: 20px;
}
// .nav-links {
//   display: flex;
//   height: 50px;
//   margin-left: 20px;
// }
header nav .nav-link {
  display: flex;
  align-items: center;
  padding: 0px 15px;
  text-decoration: none;
  color: #72CE27;
  font-weight: 600;
  border-radius: px;
  margin: 5px;

}
.dark header nav .nav-link {
  color: #ADB5BD;
  border: 0.5px solid #72EFDD;
border-radius: 6px;
  font-family: 'Montserrat', sans-serif;
  // border: white 1px solid;
}
header nav .nav-link:hover {
  color: #FDD54F;
  background: #F8049C;
  // border: 1px solid #9D4EDD;
border-radius: 6px;


}
.dark header nav .nav-link:hover {
  color: #6c757d;
  background: #72EFDD;
  // border: 0.5px solid #72EFDD;

}
// .color {
//     display: flex;
//     align-items: center;
//     // justify-content: space-around;
// }
// .toggle {
//   margin-right: 40px;
  
// }
@media screen and (max-width: 700px) {

  

  .dropdown-menu {
    $dropdown-dark-link-disabled-color: red;
    // $dropdown-color: var(--#ADB5BD body-color);
    // background: #80ffdb;
    background: linear-gradient(180deg, rgba(192,253,255,1) 0%, rgba(222,170,255,1) 100%);
    // background: linear-gradient(0deg, rgba(123,241,168,1) 0%, rgba(193,251,164,1) 25%, rgba(255,239,159,1) 50%, rgba(255,214,224,1) 75%, rgba(144,241,239,1) 100%);
    // background: url("../assets/ballons.png") no-repeat center center;

    padding: 0;
  }
.dark .dropdown-menu { 
  $dropdown-dark-link-disabled-color: #0B525B;

  background: linear-gradient( rgba(49,34,68,1) 0%, rgba(33,47,69,1) 39%, rgba(27,58,75,1) 61%, rgba(11,82,91,1) 100%);

}


  .dropdown-menu .nav-link {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  color: #212529;
  padding: 5px 10px;
  margin: 20px;
}
.dropdown-menu .nav-link:hover {
  color: #F8049C;
  font-weight: 600;

  // background: #ADB5BD;
  margin: 20px;
  border-radius: 5px;
border-bottom: 1px solid #9D4EDD;
margin: 20px;
}
.dark .dropdown-menu .nav-link {
color: #CED4DA;
font-size: 18px;
margin: 20px;
}
.dark .dropdown-menu .nav-link:hover {
  color: #80FFDB;
  font-weight: 600;
  // background: #ADB5BD;
  margin: 0px 25px;
  border-radius: 5px;
border-bottom: none;

  // border: 0.5px solid #70E000;
  margin: 20px;
}
  .dropdown {
  display: contents;
  margin-right: 60px;
}
header nav {
  display: none;
}
header h1 {
  font-size: 25px;
}
}
</style>