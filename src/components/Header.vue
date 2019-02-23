<template>
    <div>
    <!-- Menu Content -->
    <header id="nav-header">
      <div class="main-nav">
        <h1 class="logo"><a class="logo" href="index.html">S&J</a></h1>
        <div class="menu-btn" v-on:click="open">
          <div class="btn-line"></div>
          <div class="btn-line"></div>
          <div class="btn-line"></div>
        </div>
      </div>
      <!-- <p class="btn-container"><button class="nav-btn">click</button></p> -->
      <nav class="nav-container">
        <div ref="navHide" class="nav-links hide">
            <router-link to="/"><a class="nav-link nav-text">Home</a></router-link> 
            <router-link to="/services"><a class="nav-link nav-text">Services</a></router-link> 
            <router-link to="/contact"><a class="nav-link nav-text">Contact</a></router-link> 
        </div>
      </nav>
    </header>
    </div>
</template>

<script>
export default {
    name: "Header",
    methods: {
        open: function (e){
            this.$refs.navHide.classList.toggle('hide');
        }
    }
}

</script>

<style scoped>

</style>

