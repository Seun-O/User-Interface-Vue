<template>
  <div id="app">
    <!-- <Header /> -->
    <router-view/>
    <Footer />
  </div>
</template>


<script>
import Header from "./components/Header"
import Footer from "./components/Footer"

export default {
  name: 'app',
  components:{
    Header,
    Footer,
  }
}
</script>


<style>
/* http://meyerweb.com/eric/tools/css/reset/  */
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, figcaption, figure,
footer, header, hgroup, menu, nav, section, summary,
time, mark, audio, video {
  margin: 0;
  padding: 0;
  border: 0;
  outline: 0;
  font-size: 100%;
}
/* HTML5 display-role reset for older browsers */
body {
  line-height: 1;
}

table {
  border-spacing: 0;
}
/* Your Code Goes Here */
.jumbo {
  font-weight: bold;
  font-size: 6.4rem;
  line-height: 7.5rem;
  color: #ffffff;
}

.sub {
  font-weight: bold;
  font-size: 2.8rem;
  color: #222222;
  margin-bottom: 1rem;
}

.ft-head {
  font-weight: regular;
  font-size: 2rem;
  line-height: 2.4rem;
  color: #ffffff;
}

.ft-text {
  font-weight: regular;
  font-size: 1.3rem;
  line-height: 2.6rem;
  color: #ffffff;
}

.logo {
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

.btn {
  margin: 2rem 0;
  padding: 1.6rem 5rem;
  background: #ffffff;
  border: 1px solid;
  cursor: pointer;
  outline: none;
  font-family: Roboto, Arial, sans-serif;
}
.btn.learn:hover {
  background: #5e9fb9;
  color: #ffffff;
}
.btn.link {
  font-size: 3rem;
}
.btn.link:hover {
  color: #ffffff;
  background: #222222;
}
.btn.active-tab {
  background: #5e9fb9;
  color: #ffffff;
}

@keyframes animat_show {
  0% {
    opacity: 0;
    transform: translateY(-100px);
  }
  100% {
    opacity: 1;
    transform: translateY(0px);
  }
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
/* #nav-header .main-nav .menu-btn.close {
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
} */
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
}

html {
  height: 100%;
  font-size: 62.5%;
  scroll-behavior: smooth;
}

body {
  width: 100%;
  margin: 0 auto;
  font-family: Roboto, Arial, sans-serif;
  color: #222222;
}

p {
  font-size: 1.8rem;
  line-height: 2.6rem;
}

#main-header .bg {
  background-image: url("assets/home/home-jumbotron.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
  margin: 0 0 3rem 0;
}
#main-header .bg a {
  text-decoration: none;
}
#main-header .bg .bg-arrow {
  display: flex;
  justify-content: center;
  align-content: flex-end;
  text-decoration: none;
  font-size: 4.2rem;
}
#main-header .bg .bg-arrow i {
  color: white;
}
#main-header .bg .jumbo {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  height: 80%;
}
#main-header .bg .jumbo h2 {
  padding: 0 0 0 3rem;
}

#main {
  margin: 0 4rem 4rem 4rem;
  padding: 0 4rem;
}
#main .section {
  display: flex;
  padding: 4rem;
}
#main .section .text-content {
  width: 50%;
  align-self: center;
  /* align-self-margin: 0 0 4rem 0; */
}
#main .section .img-content {
  width: 50%;
  padding: 2rem;
}
#main .section .img-content img {
  max-width: 100%;
  width: 80%;
  margin: 0 0 2rem 0;
}
#main #projects {
  padding: 0 4rem;
}
#main #projects .project {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 4rem 0;
}
#main #projects .project .project-text {
  width: 50%;
  margin: 2rem 0;
  line-height: 5rem;
}
#main #projects .project-head {
  display: flex;
  flex-direction: column;
}
#main #projects .project-head img {
  width: 100%;
}
#main #projects .project-head h2 {
  background: #d8d8d8;
  text-align: center;
  width: 25%;
  padding: 2rem 1rem;
  margin-top: -3rem;
  margin-bottom: 3rem;
  z-index: 99;
}
#main #projects .project-1 .project-head {
  align-items: flex-end;
}
#main #projects .project-2 .project-head {
  align-items: flex-start;
}
#main #projects .project-3 .project-head {
  align-items: flex-end;
}

.service-head img {
  width: 100%;
  max-width: 100%;
}
.service-head img.mobile-img {
  display: none;
}
.service-head h2 {
  margin: -10rem 0 5rem 5rem;
}

#services {
  padding: 0 4rem;
  margin: 0 4rem 4rem 4rem;
}
#services .tab-links {
  display: flex;
  justify-content: space-between;
}
#services .tab-content {
  display: flex;
  justify-content: space-between;
  width: 100%;
  margin: 0 4rem;
}
#services .tab-content .tab-text {
  width: 50%;
}
#services .tab-content .tab-img {
  width: 50%;
  text-align: center;
}
#services .tab-content .tab-img img {
  display: flex;
  display: none;
  max-width: 100%;
}
#services .tab-content .tab-img img.img-active {
  display: flex;
  margin: 0 auto;
}

.contact-head h2 {
  margin: -10rem 0 6rem 5rem;
}
.contact-head img {
  width: 100%;
  height: 20rem;
}
.contact-head img.mobile-img {
  display: none;
}

#contact {
  display: flex;
  justify-content: space-around;
  margin: 0 4rem;
}
#contact .contact-section {
  width: 50%;
  font-size: 2rem;
  margin: 0 0 0 4rem;
}
#contact .contact-section h2 {
  font-size: 3rem;
  margin-bottom: 2.6rem;
}
#contact .contact-section form {
  display: flex;
  flex-direction: column;
}
#contact .contact-section form select, #contact .contact-section form input[type=text], #contact .contact-section form input[type=email], #contact .contact-section form textarea {
  width: 50rem;
  height: 2.6rem;
  border-radius: 3px;
  outline: none;
  border: 0.5px solid lightgray;
  padding: 0.5rem;
  margin: 1rem 0 0 0;
}
#contact .contact-section form label {
  margin: 1rem 0;
}
#contact .contact-section form div {
  margin: 1rem 0;
}
#contact .contact-section form .project-summary {
  display: flex;
  flex-direction: column;
}
#contact .contact-section form .project-summary textarea {
  height: 15rem;
}
#contact .contact-section form .email-input p {
  font-size: 1.2rem;
}
#contact .contact-section form .radio-options input {
  margin: 1rem 0;
  padding: 0 2rem;
}
#contact .contact-work {
  font-size: 2rem;
  width: 30%;
}
#contact .contact-work h2 {
  font-size: 3rem;
  margin-bottom: 2.6rem;
}

.img-hide {
  visibility: hidden;
}

.fadeIn {
  -webkit-animation: animat_show 0.8s ease-out;
  animation: animat_show 0.8s ease-out;
  visibility: visible;
}

footer {
  background: #828282;
  padding: 4rem 0 0 0;
}
footer span {
  display: flex;
  justify-content: center;
  margin: 1rem 0 0 0;
}
footer .ft-flex {
  display: flex;
  justify-content: space-evenly;
}
footer .ft-connect input {
  border-radius: 3px;
  height: 10%;
  width: 98%;
  outline: none;
  border: 0;
  padding: 1rem;
}
footer .ft-connect .ft-email-container {
  display: flex;
  position: relative;
}
footer .ft-connect .ft-email-container .ft-btn {
  position: absolute;
  right: 0;
  height: 100%;
  width: 25%;
  text-align: center;
  border-radius: 0px 3px 3px 0px;
  background: #5e9fb9;
  cursor: pointer;
}
footer .ft-connect .ft-email-container .ft-btn:hover {
  background: black;
}
footer .ft-connect .ft-email-container .ft-btn i {
  font-size: 1.6rem;
  margin: 1rem 0 0 0;
}

@media screen and (max-width: 800px) {
  footer .ft-flex {
    flex-direction: column;
    padding: 0 0 0 2rem;
  }
  footer .ft-connect .ft-email-container .ft-btn {
    top: 10px;
    right: 80px;
    height: 65%;
    width: 20%;
  }
  footer .ft-connect .ft-head {
    margin: 1rem 0;
  }
  footer .ft-connect input {
    width: 70%;
    margin: 1rem 0;
  }
  footer .ft-head {
    margin: 1.6rem 0 0 0;
  }
}
@media screen and (max-width: 800px) {
  #main-header .bg {
    height: 50vh;
  }
  #main-header .bg h2 {
    padding: 0;
    font-size: 5rem;
  }

  #main {
    margin: 0;
    padding: 0;
  }
  #main .section {
    flex-direction: column;
    padding: 0;
    margin: 0;
  }
  #main .section .text-content {
    width: 100%;
  }
  #main .section .img-content {
    width: 100%;
    padding: 0;
  }
  #main .section .img-content img {
    width: 100%;
    max-width: 100%;
  }
  #main .section.intro .text-content {
    text-align: center;
    order: 1;
  }
  #main .section.intro .img-content {
    order: 0;
  }
  #main .section.designs .text-content {
    text-align: center;
  }
  #main #projects {
    padding: 0;
  }
  #main #projects .project {
    margin: 0;
  }
  #main #projects .project .project-text {
    width: 100%;
    text-align: center;
  }
  #main #projects .project .project-head h2 {
    width: 80%;
    align-items: center;
    margin-top: -2rem;
  }
  #main #projects .project-1 .project-head, #main #projects .project-2 .project-head, #main #projects .project-3 .project-head {
    align-items: center;
  }

  .service-head {
    margin: 0 0 3rem 0;
  }
  .service-head img.mobile-img {
    display: block;
  }
  .service-head img.desk-img {
    display: none;
  }

  #services {
    margin: 0 0 4rem 0;
    padding: 0 2rem;
  }
  #services .tab-links {
    text-align: center;
    flex-direction: column;
  }
  #services .tab-content {
    margin: 0;
    padding: 0;
    flex-direction: column;
  }
  #services .tab-content .tab-text {
    width: 100%;
    margin: 2rem 0;
  }
  #services .tab-content .tab-text h2 {
    margin: 0 0 2rem 0;
  }
  #services .tab-content .tab-img {
    width: 100%;
  }

  #contact {
    flex-direction: column;
    margin-bottom: 4rem;
  }
  #contact .contact-section {
    width: 100%;
    margin: 0;
  }
  #contact .contact-section form .email-input input {
    width: 30rem;
  }
  #contact .contact-section form .buildings select {
    width: 30rem;
  }
  #contact .contact-section form .project-summary textarea {
    width: 30rem;
  }
  #contact .contact-section form .submit-container .btn {
    width: 100%;
    justify-self: center;
  }
  #contact .contact-work {
    width: 100%;
  }
  #contact .contact-work input {
    width: 20rem;
  }
}

/*# sourceMappingURL=index.css.map */

</style>
