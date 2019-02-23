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
            <router-link to="/about"><a class="nav-link nav-text">Services</a></router-link> 
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
/* .logo {
  font-weight: bold;
  font-size: 2.4rem;
  color: #ffffff;
  text-decoration: none;
}

.nav-text {
  font-weight: bold;
  font-size: 4.8rem;
  line-height: 8.5rem;
  color: #ffffff;
}
#nav-header {
  background: #a9b3bd;
  padding: 2rem 0;
  width: 100%;
}
#nav-header .main-nav {
  background: #a9b3bd;
  display: flex;
  width: 100%;
  justify-content: space-between;
  align-items: center;
}
#nav-header .main-nav .logo {
  margin: 0 4rem;
}
#nav-header .main-nav .menu-btn {
  z-index: 999;
  cursor: pointer;
  margin: 0 4rem;
}
#nav-header .main-nav .menu-btn .btn-line {
  width: 28px;
  height: 3px;
  margin-bottom: 5px;
  background: #ffffff;
}
#nav-header .main-nav .menu-btn.close {
  transform: rotate(180deg);
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
#nav-header .nav-container {
  display: flex;
  justify-content: center;
}
#nav-header .nav-container .nav-links {
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  height: 100vh;
}
#nav-header .nav-container .nav-links.hide {
  display: none;
}
#nav-header .nav-container .nav-links a {
  text-decoration: none;
}
#nav-header .nav-container .nav-links a:hover {
  color: #222222;
} */
</style>

