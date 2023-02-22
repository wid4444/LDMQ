<template>

    <header>

        <h1>
            Leobardo D. Martinez-Quiroz
        </h1>
        
        <nav>
            <router-link class="nav-link" :mode="mode" to="/">Home</router-link>
            <router-link class="nav-link" :mode="mode" to="/about">About</router-link>
            <router-link class="nav-link" :mode="mode" to="/portfolio">Portfolio</router-link>
            <router-link class="nav-link" :mode="mode" to="/contact">Contact</router-link>

            <!-- <div class="nav-link">Portfolio</div>
            <div class="nav-link">Contact</div> -->

            <!-- <HamburgerMenu :mode="mode" /> -->

        </nav>

        <div class="color">
            <h1>{{ mode }} Mode</h1>

            <div class="toggle">
                <Toggle :mode="mode" @toggle="$emit('toggle')" />
            </div>
        </div>

    </header>
</template>


<script>
// @ is an alias to /src
import Toggle from '@/components/Toggle.vue'
import Content from '@/components/Content.vue'
// import HamburgerMenu from './HamburgerMenu.vue'


export default {
props: ['mode'],
components: {
  Toggle,
  Content,
//   HamburgerMenu,

  
}
}
</script>



<style scope lang="scss">
* {
  font-family: 'Montserrat', sans-serif;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: opx 25px;
  height: 60px;
  background: #C3C3C3;
  transition: background 0.3s ease-in-out;
}
.dark header {
  background: #1d1d1d;
}
header h1 {
    font-family: 'Montserrat', sans-serif;
  font-size: 15px;
//   text-transform: uppercase;
//   font-weight: 600;
  margin-left: 20px;

}
.color h1 {
    margin-right: 20px;
  text-transform: uppercase;

}
header nav {
  display: flex;
  height: 50px;
  margin-left: 20px;
}
header nav .nav-link {
  display: flex;
  align-items: center;
  padding: 0px 15px;
  text-decoration: none;
  color: #212529;
  font-weight: 600;
  // border: 1px solid black;
  border-radius: 5px;
  margin: 5px;

}
.dark header nav .nav-link {
  color: #B0B0B0;
  // border: white 1px solid;
}
header nav .nav-link:hover {
  background: #6c757d;
}
.dark header nav .nav-link:hover {
  background: #6c757d;
}
.color {
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.toggle {
  margin-right: 40px;
  
}

</style>