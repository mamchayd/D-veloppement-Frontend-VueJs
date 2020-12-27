<template>
<div class="container">
<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a class="navbar-item" href="#">
      <img  :src="logo">
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-start">
      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link">
          Best places
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item">
            Montain
          </a>
          <a class="navbar-item">
            Beaches
          </a>
          <a class="navbar-item">
            Sahara
          </a>
        </div>
      </div>

      <div class="navbar-item has-dropdown is-hoverable">
        <a class="navbar-link">
          Destinations
        </a>

        <div class="navbar-dropdown">
          <a class="navbar-item">
            Agadir-Taghazout
          </a>
          <a class="navbar-item">
            Al Hoceima
          </a>
          <a class="navbar-item">
            Azilal
          </a>
          <a class="navbar-item">
            Casablanca
          </a>
          <a class="navbar-item">
            Errachidia-Midelt -Merzouga
          </a>  
          <a class="navbar-item">
            Fès-Meknès
          </a> 
          <a class="navbar-item">
            Essaouira-Mogador
          </a>           
                  
          
          
        </div>
      </div>
      <a class="navbar-item">
        Cuisine marocaine
      </a>
      <a class="navbar-item">
        Trips
      </a>
      <a class="navbar-item">
        Blog
      </a>
      <a class="navbar-item">
        Resources
      </a>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">
          <a class="button signup">
            <strong>Sign up</strong>
          </a>
          <a class="button is-light">
            Log in
          </a>
        </div>
      </div>
    </div>
  </div>
</nav>
</div>
</template>

<script>
export default {
  name: "Header",
    data: function(){
        return {
        logo:""
        }
    },

    created: function() {
    this.logo = "./images/logo.png";
    }
}
</script>

<style>
.navbar-item img {
  height: 50px;
  max-height: 50px !important;
}
.buttons .signup {
  background: #FE6103;
  color: #fff;
}
</style>