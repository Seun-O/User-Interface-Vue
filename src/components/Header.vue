<template>
    <div>
    <!-- Menu Content -->
    <header id="nav-header">
      <div class="main-nav">
        <h1 class="logo"><a class="logo" href="index.html">S&J</a></h1>
        <div ref="menuBtn" class="menu-btn" v-on:click="open">
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
            this.$refs.menuBtn.classList.toggle('close');
        }
    }
}

</script>

<style scoped>
.menu-btn{
    transition: ease-out 0.5s;
}
#nav-header .main-nav .menu-btn.close {
  transform: rotate(90deg);
}
#nav-header .main-nav .menu-btn.close .btn-line:nth-child(1) {
  transform: rotate(45deg) translate(5px, 5px);
}
#nav-header .main-nav .menu-btn.close .btn-line:nth-child(2) {
  opacity: 0;
}
#nav-header .main-nav .menu-btn.close .btn-line:nth-child(3) {
  transform: rotate(-45deg) translate(7px, -6px);
}
</style>

