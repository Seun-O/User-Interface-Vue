<template>
  <div>
    <Header />
      <div class="service-head">
      <img class="desk-img" src="../assets/services/services-jumbotron.png" alt="" />
      <img
        class="mobile-img"
        src="../assets/services/services-mobile-jumbotron.png"
        alt=""
      />
      <h2 class="jumbo">Services</h2>
    </div>

    <section id="services">
      <div class="services-intro">
        <p>
          Services include: completely synergize resource taxing relationships
          via premier niche markets. Professionally cultivate one-to-one
          customer service with robust ideas. Dynamically innovate
          resource-leveling customer service for state of the art customer
          service.
        </p>
      <!-- <Slider /> -->
      </div>
      <Tabs />
    </section>
  </div>
</template>

<script>
import Header from "../components/Header"
import Tabs from "../components/Tabs"
import Slider from "../components/Slider"
export default {
  name: "Services",
  components: {
    Tabs,
    Slider,
    Header,
  }
}
</script>
