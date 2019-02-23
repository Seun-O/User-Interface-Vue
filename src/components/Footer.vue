<template>
    <div>
    <!-- FOOTER CONTENT -->
    <footer class="ft-text">
      <div class="ft-flex">
        <div class="ft-connect">
          <h2 class="ft-head">
            Interested in starting a project?<br />
            Let’s talk:
          </h2>
          <div class="ft-email-container">
            <input type="email" placeholder="Enter email" />
            <div class="ft-btn"><i class="fas fa-envelope"></i></div>
          </div>
          <br />
          We'll never share your email with anyone else.
        </div>

        <div>
          <h2 class="ft-head">New York</h2>
          123 Lane<br />
          Suite 100<br />
          Albany, NY 12345<br />
          202 555 0144
        </div>

        <div>
          <h2 class="ft-head">Florida</h2>
          Ocean Drive<br />
          Suite 201<br />
          Orlando, FL 22345<br />
          502 555 0144
        </div>

        <div>
          <h2 class="ft-head">California</h2>
          Mountain Street<br />
          Suite 105<br />
          San Diego, CA 22345<br />
          702 555 0144<br />
        </div>
      </div>
      <span>Copyright © 2018 Smith and Jones</span>
    </footer>
    </div>
</template>

<script>
export default {
    name: "Footer"
}
</script>


<style scoped>
/* footer {
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
} */
</style>
