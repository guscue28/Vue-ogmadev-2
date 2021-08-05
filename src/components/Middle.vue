<template>
  <div id="mid1">
    <b-row class="text-center">
      <h1 id="title" class="mt-5 primary-text">Services</h1>
    </b-row>
    <br />
    <b-row class="text-center">
      <b-col>
        <div>
          <a v-b-modal.modal-1
            ><img
              class="objetos"
              src="https://ogma.dev/_nuxt/img/web-avatar.5780ee5.png"
              alt="Web"
          /></a>
          <b-modal ref="modal-1" id="modal-1" hide-footer hide-header>
            <b-row>
              <div id="rows">
                <h5 class="text-center">Web</h5>
                <p>
                  Web Full service for development of static or dynamic
                  websites. Solutions for the web design that you are looking
                  for.
                </p>
              </div>

              <h4 class="mt-4" style="color: #5100d1;">Technologies</h4>
              <br /><br /><br />
              <b-col>
                <h5 class="primary-text text-center">Frontend</h5>
                <br />
                <p class="text-center" style="font-size:14px;">
                  Vue.js
                  <br /><br />
                  Nuxt.js
                  <br /><br />
                  Wordpress
                </p>
              </b-col>
              <b-col>
                <h5 class="primary-text text-center">Backend</h5>
                <br />
                <div style="display:flex;  justify-content: center;">
                  <p style="font-size: 12px; ">
                    Node.js with ApiGraph
                    <br /><br />
                    Node.js with ApiRest
                    <br /><br />
                    NoSql implemend with
                    <br />
                    mongo DB y
                    <br />
                    Mongoose
                  </p>
                </div>
              </b-col>
              <div></div>
              <br /><br /><br /><br /><br /><br /><br /><br />
              <div style="display: flex; justify-content: center;">
                <b-button
                  href="#"
                  style=" width: 160px; height: 35px; border-radius: 15px; background: #5100d1; color: white;"
                  v-scroll-to="{ el: '#vlow', offset: -60 }"
                  @click="hideModal()"
                  >CONTACT US</b-button
                >
              </div>
            </b-row>
          </b-modal>
        </div>
        <br />
        <h5 class="text">Web</h5>
      </b-col>
      <b-col>
        <div>
          <a v-b-modal.modal-2
            ><img
              class="objetos"
              src="https://ogma.dev/_nuxt/img/app-avatar.14d2638.png"
              alt="App"
          /></a>
          <b-modal ref="modal-2" id="modal-2" hide-footer hide-header>
            <b-row>
              <div id="rows">
                <h5 class="text-center">App</h5>
                <p style="text-align: justify;">
                  The app you have in mind, we can make it real. We bring new
                  technologies and the most dedicated team for iOS & Android app
                  mobile development. In the Ogma team we adapt ourselves to the
                  needs of the client achieving high quality & profitable
                  products. Additionally we focus on UX and UI for intuitive
                  navigation that allows positive user experience.
                </p>
              </div>

              <h4 class="mt-4" style="color: #5100d1;">Technologies</h4>
              <br /><br /><br />
              <b-col>
                <h5 class="primary-text text-center">Frontend</h5>
                <br />
                <p class="text-center" style="font-size: 14px;">
                  React Native
                  <br /><br />
                  Ionic
                </p></b-col
              >

              <b-col>
                <h5 class="primary-text text-center">Backend</h5>
                <br />
                <div style="display:flex;  justify-content: center;">
                  <p style="font-size: 12px; ">
                    Node.js with ApiGraph
                    <br /><br />
                    Node.js with ApiRest
                    <br /><br />
                    NoSql implemend with
                    <br />
                    mongo DB y
                    <br />
                    Mongoose
                  </p>
                </div>
              </b-col>
              <div></div>
              <br /><br /><br /><br /><br /><br /><br /><br />

              <div style="display: flex; justify-content: center;">
                <b-button
                  href="#"
                  style=" width: 160px; height: 35px; border-radius: 15px; background: #5100d1; color: white;"
                  v-scroll-to="{ el: '#vlow', offset: -60 }"
                  @click="hideModal()"
                  >CONTACT US</b-button
                >
              </div>
            </b-row>
          </b-modal>
        </div>
        <br />
        <h5 class="text">App</h5>
      </b-col>
      <b-col>
        <div>
          <a v-b-modal.modal-3
            ><img
              class="objetos"
              src="https://ogma.dev/_nuxt/img/desk-avatar.8d26e72.png"
              alt="Desk"
          /></a>
          <b-modal ref="modal-3" id="modal-3" hide-footer hide-header>
            <b-row>
              <div id="rows">
                <h5 class="text-center">Desk</h5>
                <p style="text-align: justify;">
                  Desktop applications offer solutions to business needs and
                  complex problems. Our service is oriented to cover a wide
                  range of different requirements of our clients so that desktop
                  applications elevate the experience of organization and
                  customizable management
                </p>
              </div>

              <h4 class="mt-4" style="color: #5100d1;">Technologies</h4>
              <br /><br /><br />
              <b-col>
                <h5 class="primary-text text-center">Frontend</h5>
                <br />
                <p class="text-center" style="font-size: 14px;">
                  Electron
                  <br /><br />
                  C++
                </p></b-col
              >
              <b-col>
                <h5 class="primary-text text-center">Backend</h5>
                <br />
                <div style="display:flex;  justify-content: center;">
                  <p style="font-size: 12px; ">
                    Node.js with ApiGraph
                    <br /><br />
                    Node.js with ApiRest
                    <br /><br />
                    NoSql implemend with
                    <br />
                    mongo DB y
                    <br />
                    Mongoose
                  </p>
                </div>
              </b-col>
              <div></div>
              <br /><br /><br /><br /><br /><br /><br /><br />

              <div style="display: flex; justify-content: center;">
                <b-button
                  href="#"
                  style=" width: 160px; height: 35px; border-radius: 15px; background: #5100d1; color: white;"
                  v-scroll-to="{ el: '#vlow', offset: -60 }"
                  @click="hideModal()"
                  >CONTACT US</b-button
                >
              </div>
            </b-row>
          </b-modal>
        </div>
        <p>Desk</p>
      </b-col>
      <b-col>
        <div>
          <a v-b-modal.modal-4
            ><img
              class="objetos"
              src="https://ogma.dev/_nuxt/img/e-commerce-avatar.75bfdf3.png"
              alt="E-commerce"
          /></a>
          <b-modal ref="modal-4" id="modal-4" hide-footer hide-header>
            <b-row>
              <div id="rows">
                <h5 class="text-center">E-commerce</h5>
                <p style="text-align: justify;">
                  The business world is changing at a breakneck pace where
                  everything is digitized. Having an e‐commerce is a determining
                  factor to increase the profitability and sales of your
                  business.
                </p>
              </div>

              <h4 class="mt-4" style="color: #5100d1;">Technologies</h4>
              <br /><br /><br />
              <b-col>
                <h5 class="primary-text text-center">Frontend</h5>
                <br />
                <p class="text-center" style="font-size: 14px;">
                  ---------
                  <br /><br />
                  Shopify
                  <br /><br />
                  Prestashop
                </p></b-col
              >

              <b-col>
                <h5 class="primary-text text-center">Backend</h5>
                <br />
                <div style="display:flex;  justify-content: center;">
                  <p style="font-size: 12px; ">
                    Node.js with ApiGraph
                    <br /><br />
                    Node.js with ApiRest
                    <br /><br />
                    NoSql implemend with
                    <br />
                    mongo DB y
                    <br />
                    Mongoose
                  </p>
                </div>
              </b-col>
              <div></div>
              <br /><br /><br /><br /><br /><br /><br /><br />

              <div style="display: flex; justify-content: center;">
                <b-button
                  href="#"
                  class="mt-8"
                  style=" width: 160px; height: 35px; border-radius: 15px; background: #5100d1; color: white;"
                  v-scroll-to="{ el: '#vlow', offset: -60 }"
                  @click="hideModal()"
                  >CONTACT US</b-button
                >
              </div>
            </b-row>
          </b-modal>
        </div>
        <p>E-commerce</p>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: "Middle",
  methods: {
    hideModal() {
      this.$refs["modal-1"].hide();
      this.$refs["modal-2"].hide();
      this.$refs["modal-3"].hide();
      this.$refs["modal-4"].hide();
    },
  },
};
</script>

<style>
#mid1 {
  width: 100%;
}

.objetos {
  height: 140px;
  min-width: 140px;
  width: 140px;
  border: 0px solid rgb(227, 227, 227);
  cursor: pointer;
}

.objetos:hover {
  transition: 1s;
  width: 135px;
  height: 135px;
  border-radius: 100%;
  border: 3px solid rgb(227, 227, 227);
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.5);
}

#modal1 {
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  border-radius: 15px;
  display: flex;
  flex-direction: column;
}

#rows {
  text-align: justify;
  font-family: sans-serif;
  background: #5100d1;
  color: white;
}
</style>
