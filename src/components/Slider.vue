<template>
    <div>
      <div class="slider">
        <div class="slide-image fade">
          <div class="numbertext"></div>
          <img src="../assets/home/home-outskirts-img.png" />
          <div class="text">The Outskirts</div>
        </div>

        <div class="slide-image fade">
          <div class="numbertext"></div>
          <img src="../assets/home/home-the-blocks-img.png" />
          <div class="text">The Blocks</div>
        </div>

        <div class="slide-image fade">
          <div class="numbertext"></div>
          <img src="../assets/home/home-villas-img.png" />
          <div class="text">The Villas</div>
        </div>

        <p class="prev">&#10094;&#10094;</p>
        <p class="next">&#10095;&#10095;</p>

        <div class="dot-container"></div>
      </div>
    </div>
</template>

<script>
export default {
    name: "Slider"
}
</script>

<style scoped>
.slide-image {
  display: none;
}
/* Slideshow container */
.slider {
  max-width: 1000px;
  position: relative;
  margin: auto;
}
.slider img {
  vertical-align: middle;
  width: 100%;
}

/* Next & previous buttons */
.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
  background-color: rgba(0, 0, 0, 0.3);
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.9);
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 2.8rem;
  padding: 1.7rem 0;
  position: absolute;
  bottom: 9.4rem;
  width: 100%;
  text-align: center;
  background: rgba(0, 0, 0, 0.8);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
  background-color: rgba(0, 0, 0, 0.8);
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.dot-container {
  text-align: center;
  margin: -3.5rem 0 3rem 0;
}

.active,
.dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {
    opacity: 0.4;
  }
  to {
    opacity: 1;
  }
}
@keyframes fade {
  from {
    opacity: 0.4;
  }
  to {
    opacity: 1;
  }
}
/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev,
.next,
.text {
    font-size: 11px;
  }
}
@media screen and (max-width: 800px) {
  .text {
    color: #f2f2f2;
    font-size: 15px;
    padding: 8px 0;
    position: absolute;
    bottom: 18px;
    width: 100%;
    text-align: center;
    background: rgba(0, 0, 0, 0.8);
  }

  .dot-container {
    text-align: center;
    margin: -2rem 0 3rem 0;
  }
}
</style>
