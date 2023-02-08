<template>
    <header>

        <nav>
            <router-link class="nav-link" :mode="mode" to="/">Home</router-link>
            <router-link class="nav-link" :mode="mode" to="/about">About</router-link>
            <div class="nav-link">Portfolio</div>
            <div class="nav-link">Contact</div>
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


export default {
props: ['mode'],
components: {
  Toggle,
  Content,

  
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
  background: #15202B;
}
header h1 {
  font-size: 15px;
  text-transform: uppercase;
  font-weight: 600;
  margin-right: 20px;

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
  color: #15202B;
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