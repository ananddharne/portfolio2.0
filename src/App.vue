

<template>
  <div id="app">


<!-- <div id = "navbar">
<aside class="menu">
    <ul>
 <li><router-link to  = "#"> Home </router-link></li>
<li><router-link to  = "/skills"> Skills </router-link></li>
<li><router-link to  = "/work"> Work </router-link></li>
<li><router-link to  = "/Contact"> Contact </router-link></li>
</ul>

</aside>
 </div>   -->

   

  <nav class="nav has-shadow">
  <div class="container">
    <div class="nav-left">
      <a class="nav-item">
        <img src="http://bulma.io/images/bulma-logo.png" alt="Bulma logo">
      </a>

      <a class="nav-item is-tab is-hidden-mobile is-active"> <router-link to  = "/Home"> Home </router-link></a>
      <a class="nav-item is-tab is-hidden-mobile"><router-link to  = "/about"> About </router-link></a>
      <a class="nav-item is-tab is-hidden-mobile"> <router-link to  = "/skills">Skills</router-link></a>
      <a class="nav-item is-tab is-hidden-mobile"> <router-link to  = "/work">Work</router-link></a>
      <a class="nav-item is-tab is-hidden-mobile"> <router-link to  = "/contact">Contact </router-link></a>
    </div>
    <span class="nav-toggle">
      <span></span>
      <span></span>
      <span></span>
    </span>
    <div class="nav-right nav-menu">
      <a class="nav-item is-tab is-hidden-tablet is-active">Home</a>
      <a class="nav-item is-tab is-hidden-tablet">About</a>
      <a class="nav-item is-tab is-hidden-tablet">Skills</a>
      <a class="nav-item is-tab is-hidden-tablet">Work</a> 
      <a class="nav-item is-tab is-hidden-tablet">Contact</a>
      <a class="nav-item is-tab">
      <span class="icon">
        <i class="fa fa-github"></i>
      </span>
    </a>
   <a class="nav-item">
      <span class="icon" >
        <i class="fa fa-twitter"></i>
      </span>
    </a>

 <a class="nav-item">
      <span class="icon">
        <i class="fa fa-linkedin"></i>
      </span>
    </a>

    </div>
  </div>
</nav>

<div id="particles-js"> 

</div>

   <div> <router-view></router-view> </div>

  </div>




</template>

<script>
/* eslint-disable */


import particles from 'particles.js'

export default {
  name: 'app',
mounted () {
    this.$nextTick(() => {
      this.initParticleJS() 
    })
    
  },
  methods: {
    initParticleJS () {
      particlesJS('particles-js', {
          "particles": {
            "number": {
              "value": 80,
              "density": {
                "enable": true,
                "value_area": 800
              }
            },
            "color": {
              "value": "#192231"
            },
            "shape": {
              "type": "circle",
              "stroke": {
                "width": 0,
                "color": "#192231"
              },
              "polygon": {
                "nb_sides": 5
              }
            },
            "opacity": {
              "value": 0.6,
              "random": false,
              "anim": {
                "enable": false,
                "speed": 1,
                "opacity_min": 0.1,
                "sync": false
              }
            },
            "size": {
              "value": 3,
              "random": true,
              "anim": {
                "enable": false,
                "speed": 40,
                "size_min": 0.1,
                "sync": false
              }
            },
            "line_linked": {
              "enable": true,
              "distance": 150,
              "color": "#ffffff",
              "opacity": 0.4,
              "width": 1
            },
            "move": {
              "enable": true,
              "speed": 6,
              "direction": "none",
              "random": false,
              "straight": false,
              "out_mode": "out",
              "bounce": false,
              "attract": {
                "enable": false,
                "rotateX": 600,
                "rotateY": 1200
              }
            }
              },
              "interactivity": {
            "detect_on": "canvas",
            "events": {
              "onhover": {
                "enable": true,
                "mode": "grab"
              },
              "onclick": {
                "enable": true,
                "mode": "push"
              },
              "onresize":{ 

                "enable": true,
        "density_auto": true,
        "density_area": 400

              }
            },
            "modes": {
              "grab": {
                "distance": 140,
                "line_linked": {
                  "opacity": 1
                }
              },
              "bubble": {
                "distance": 400,
                "size": 40,
                "duration": 2,
                "opacity": 8,
                "speed": 3
              },
              "repulse": {
                "distance": 200,
                "duration": 0.4
              },
              "push": {
                "particles_nb": 4
              },
              "remove": {
                "particles_nb": 2
              }
            }
          },
          "retina_detect": true
        });
    }


  
}


  }



    /* eslint-disable */

</script>


 
<style>

#app {
  

height: 100%;



}

/*#particles-js {
    width: 100%;
    height: 100%;
    position: fixed;
    z-index: -10;
    top: 0;
    left: 0
}*/

canvas {
  display: block;
  vertical-align: bottom;
 
 background-color: #494e6b ;
}


li{
    margin-top: 30px;
    
    object-position: 
}

.has-shadow {


 
background-color: #192231;
  
}


 
</style>

