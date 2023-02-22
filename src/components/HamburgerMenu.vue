<template>
    <div class="header">

        <div class="nav-menu">

    <div class="logo">
                <img id="logo" src="../assets/logo.png" alt="logo">
               
            </div>

            <div class="burger">
                <i class="fas fa-bars" @click="showMenu()"></i>
            </div>

            
        </div>

        <div class="nav-content" :class="this.showMobileMenu ? 'open-menu' : 'closed-menu'">

            <ul class="nav-items">
                <li class="nav-item">
                    <router-link class="nav-link" @click="showMenu()" to="/">Home</router-link>
                </li>
                <li class="nav-item">
                    <router-link class="nav-link" @click="showMenu()" to="/about">About Us</router-link>
                </li>
                
            </ul>


        </div>
    </div>
</template>

<script>

export default {
    data() {
        return {
            showMobileMenu: false,
        };
    },
    methods: {
        showMenu() {
            this.showMobileMenu = !this.showMobileMenu;
        },
    },
};
</script>




<style lang="scss" scoped>
// @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;800&display=swap');
// .header {
//   // Will make an image background
//   background: url("../assets/main2.jpg") no-repeat center center
//     fixed;
//   -webkit-background-size: cover;
//   -moz-background-size: cover;
//   -o-background-size: cover;
//   background-size: cover;
//   // ---> Settings for Background Image
//   display: flex;
//   flex-direction: column;
//   justify-content: center;
//   align-items: center;
//   max-width: 100%;
  
// }

* {
    padding: 0;
    margin: 0;
    border: 0;
    outline: 0;
    list-style: none;
    text-decoration: none;
}

.nav-menu {
    justify-content: space-between;
    align-items: center;
    padding: 0 50px;
    height: 100px;
    display: flex;
    // background: #004B23;
    min-height: 50px;
    // opacity: 50%;
    overflow: hidden;
}

.burger {
    margin-bottom: 30px;
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    font-style: oblique;
    padding-right: 30px;
}

.nav-link {
    font-family: 'Montserrat', sans-serif;
    font-weight: 1200;
    color: #0D1F22;
    font-size: 17px;
    text-decoration: none;
    text-align: center;
    transition: all 0.3s ease 0s;
    padding: 2px 10px;
    border-radius: 20px;
    list-style: none;
    display: block;
}

.nav-link:hover {
    padding: 5px 10px;
    text-align: center;
    text-decoration: none;
    transition: 0.5s;
    background-size: 200% auto;
    color: white;
    font-size: 17px;
    border-radius: 30px;
    display: block;
    border: 0px;
    font-weight: 700;
    // box-shadow: 0px 0px 14px -7px #b100e8;
    background-image: linear-gradient(45deg, #38B000 0%, #006400 51%, #38B000 100%);
    cursor: pointer;
    user-select: none;
    -webkit-user-select: none;
    touch-action: manipulation;

}
#app {
        
        // padding-left: 600px;
    }
    .btn {
  padding: 0 15px;
  color: white;
  background: #4AAE9B;
  border: 1px solid #4AAE9B;
  border-radius: 30px;
  position: relative;
  top: 0;
  right: 0;
  border: none;
  font-size: 20px;
  margin: 10px 20px;
  cursor: pointer;
  font-weight: bold;
}

#logo {
    height: 110px;
    margin-top: 20px;
    border-radius: 10px;
}

.nav-content {
    background: transparent;
    // background: #007200;
    // opacity: 50%;
    // max-height: 80px;
    border-bottom: 3px solid green;
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    height: 100px;
}

.nav-items {
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    // margin: 10px;
    padding: 0;
    font-weight: 600;

    li {
        padding: 0 10px;
    }
}

.nav-item {
    margin: 10px 0;
}

i {
    text-align: right;
    display: none;
    color: #38B000;
    font-size: 50px;
    // opacity: 100%;

}
// Ipad size
// @media screen and (max-width:1024px) {

    
//     .nav-menu {
//         padding: 0 20px;
//     }

//     .nav-link {
//         display: flex;
//         font-family: 'Montserrat', sans-serif;
//         font-weight: 600;
//         color: white;
//         font-size: 12px;
//         text-decoration: none;
//         text-align: center;
//         transition: all 0.3s ease 0s;
//         padding: 2px 5px;
//         border-radius: 20px;
//         list-style: none;
//         text-align: center;
//         align-items: center;
//         justify-content: center;

//     }

//     .nav-link:hover {
//         padding: 4px 10px;
//         text-align: center;
//         text-decoration: none;
//         transition: 0.5s;
//         background-size: 200% auto;
//         color: white;
//         border-radius: 30px;
//         display: block;
//         border: 0px;
//         font-weight: 700;
//         box-shadow: 0px 0px 14px -7px #b100e8;
//         background-image: linear-gradient(45deg, #d300f4 0%, #b100e8 51%, #d300f4 100%);
//         cursor: pointer;
//         user-select: none;
//         -webkit-user-select: none;
//         touch-action: manipulation;

//     }
// }

// Mobile version - hidden hamburger menu

@media screen and (max-width: 700px) {          
   
    #app {
        display: none;
        padding-left: 100px;
    }
    .btn {
  padding: 0 15px;
  color: white;
  background: #4AAE9B;
  border: 1px solid #4AAE9B;
  border-radius: 30px;
  position: relative;
  top: 0;
  right: 0;
  border: none;
  font-size: 40px;
  margin: 10px 200px;
  cursor: pointer;
  font-weight: bold;
}

    #logo {
        height: 100px;
        margin-top: 0px;
        margin-left: 20px;

    }

    .nav-menu {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        padding: 0;
        height: 150px;
    //     background: black;
    // opacity: 50%;
    }

    .burger {
        margin-bottom: 30px;
        display: flex;
        flex-direction: row;
        justify-content: flex-end;
        font-style: oblique;
        padding-right: 30px;
    }

    .open-menu {
        opacity: 1;
        display: flex;
        flex-direction: column;
        position: absolute;
        box-shadow: 0px 0px 14px -7px white;
        // background-image: linear-gradient(45deg, #0707e2 0%, #7c00e8 51%, #d008d6 100%);
        background: #007200;
// opacity: 10%;

        width: 100%;
        top: 0;
        left: 0;
        transform: translateY(80%);  // Brings menu down
        z-index: 1;
        transition: .4s;
        overflow: hidden;
        text-align: center;
        border-radius: 20px;
    }

    .closed-menu {
        opacity: 0;
        height: 0;
        padding: 0;
        transform: translateY(0%);
        transition: .2s;
        overflow: hidden;
    }

    .nav-link {
        font-family: 'Montserrat', sans-serif;
        font-weight: 700;
        color: #004B23;
        opacity: 100%;
        font-size: 15px;
        text-decoration: none;
        text-align: center;
        transition: all 0.3s ease 0s;
        padding: 2px 0px;
        border-radius: 20px;
        list-style: none;

    }

    .nav-link:hover {
        padding: 5px 7px;
        text-align: center;
        text-decoration: none;
        transition: 0.5s;
        background-size: 200% auto;
        color: white;
        border-radius: 30px;
        display: block;
        border: 2px solid white;
        font-weight: 700;
        // box-shadow: 0px 0px 14px -7px #c348e9;
        background-image: linear-gradient(45deg, #38B000 0%, #006400 51%, #38B000 100%);
        cursor: pointer;
        user-select: none;
        -webkit-user-select: none;
        touch-action: manipulation;

    }

    .nav-content {
        display: flex;
        flex-direction: column;
        z-index: 100;
        transition: all 0.2s ease-out;
    //     background: grey;
    // opacity: 80%;
    }

    .nav-items {
        display: flex;
        flex-direction: column;
        margin: 20px 0;

    }

    .nav-item {
        margin: 25px;
        text-align: center;

    }

    i {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        text-align: right;
        margin-top: 20px;
    }


}
</style>