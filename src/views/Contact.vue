<template>
    <div>
        <Header />
        <div class="contact-head">
      <img class="desk-img" src="../assets/contact/contact-jumbotron.png" alt="" />
      <img
        class="mobile-img"
        src="../assets/contact/contact-mobile-jumbotron.png"
        alt=""
      />
      <h2 class="jumbo">Contact Us</h2>
    </div>
        <section id="contact">
      <div class="contact-section">
        <h2 class="sub">Get In Touch</h2>

        <form action="">
          <div class="email-input">
            <label for="email">Email Address</label>
            <br/>
            <input type="email" placeholder="Enter email" />
            <br/>
            <p>We'll never share your email with anyone else.</p>
          </div>

          <div class="buildings">
            <label for="buildings"
              >How many buildings do you need planned?</label
            ><br>
            <select name="buildings" id="build-number">
              <option value="1">1</option>
              <option value="2">2</option>
              <option value="3">3</option>
              <option value="4">4</option>
              <option value="5">5</option>
            </select>
          </div>

          <div class="project-summary">
            <label for="msg"
              >Provide a brief overview of your project needs:</label
            >
            <textarea name="msg" id="msg" cols="30" rows="10"></textarea>
          </div>

          <div class="radio-options">
            <input type="radio" name="who" value="business" /> I am a small
            business<br />
            <input type="radio" name="who" value="owner" /> I am a residential
            owner<br />
            <input type="radio" name="who" value="corporation" /> I am a
            corporation
          </div>

          <div class="submit-container">
            <input class="btn learn" type="button" value="Submit" />
          </div>
        </form>
      </div>

      <div class="contact-work">
        <h2 class="sub">Where We Work</h2>
        <div>
          <h3>New York</h3>
          <p>
            123 Lane<br />
            Suite 100<br />
            Albany, NY 12345<br />
            202 555 0144
          </p>
        </div>
		<br />
		<br />
        <div>
          <h3>Florida</h3>
          <p>
            Ocean Drive<br />
            Suite 201<br />
            Orlando, FL 22345<br />
            502 555 0144
          </p>
        </div>
		<br />
		<br />
        <div>
          <h3>California</h3>
          <p>
            Mountain Street<br />
            Suite 105<br />
            San Diego, CA 22345<br />
            702 555 0144
          </p>
        </div>
      </div>
    </section>
    </div>
</template>

<script>
import Header from "../components/Header"
export default {
    name: 'Contact',
    components:{
        Header,
    }
}
</script>


<style scoped>

</style>
