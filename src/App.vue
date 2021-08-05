<template>
  <div id="#app" class="v-application v-application--is-ltr theme--light">
    <div class="v-application--wrap">
      <!-- Vista desde Mobile-->
      <div id="navigation-icon" v-if="mobileView"></div>

      <!--Vista desde Web-->
      <div v-if="!mobileView">
        <b-row>
          <b-navbar
            id="#nav"
            class="nav"
            fixed="top"
            toggleable="lg"
            type="white"
            variant="white"
          >
            <b-container>
              <b-col>
                <b-navbar-brand
                  class="home"
                  href="#"
                  v-scroll-to="{ el: '.nav' }"
                  ><img
                    alt="ogma"
                    src="https://ogma.dev/_nuxt/img/Logo.008ac63.svg"
                    width="140"
                    class="ml-12"
                /></b-navbar-brand>
              </b-col>
              <b-col></b-col>
              <b-col sm="auto">
                <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
                <b-collapse id="nav-collapse" is-nav>
                  <b-navbar-nav class="content">
                    <b-nav-item
                      href="#"
                      v-scroll-to="{ el: '#vtop', offset: -65 }"
                      class="routes-btn mx-5 hidden-sm-and-down v-btn v-btn--flat v-btn--text theme--ligth -size--default "
                      ><span class="v-btn__content">About Us</span></b-nav-item
                    >
                    <b-nav-item
                      href="#"
                      v-scroll-to="{ el: '#vmid', offset: -45 }"
                      class="routes-btn mx-5 hidden-sm-and-down v-btn v-btn--flat v-btn--text theme--ligth -size--default s"
                      ><span class="v-btn__content">Services</span></b-nav-item
                    >
                    <b-nav-item
                      href="#"
                      v-scroll-to="{ el: '#middle2', offset: -65 }"
                      class="routes-btn mx-5 hidden-sm-and-down v-btn v-btn--flat v-btn--text theme--ligth -size--default s"
                      ><span class="v-btn__content"
                        >E-commerce</span
                      ></b-nav-item
                    >
                    <b-nav-item
                      href="#"
                      v-scroll-to="{ el: '#vlow', offset: -60 }"
                      class="routes-btn mx-5 hidden-sm-and-down v-btn v-btn--flat v-btn--text theme--ligth -size--default s"
                      ><span class="v-btn__content">Contact</span></b-nav-item
                    >
                  </b-navbar-nav>
                </b-collapse>
              </b-col>
            </b-container>
          </b-navbar>
        </b-row>
      </div>
      <vhead></vhead>
      <vtop id="vtop"></vtop>
      <vmid id="vmid"></vmid><br />
      <vmid-2></vmid-2><br />
      <low id="vlow"></low>
      <vfooter></vfooter>
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Top from "./components/Top.vue";
import Middle from "./components/Middle.vue";
import Middle2 from "./components/Middle2.vue";
import Low from "./components/Low.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  data() {
    return {
      mobileView: false,
      showNav: false,
    };
  },
  components: {
    vhead: Header,
    vtop: Top,
    vmid: Middle,
    vmid2: Middle2,
    low: Low,
    vfooter: Footer,
  },
};
</script>

<style>
* {
  transition: all 0.2s ease-in-out;
  font-family: "Roboto", sans-serif;
  line-height: 1.5;
}
.theme--light .v-application {
  background: #fff;
  color: rgba(0, 0, 0, 0.87);
}
.v-application {
  font-family: "Roboto", sans-serif;
  line-height: 1.5;
  display: flex;
}
.v-application--wrap {
  flex: 1 1 auto;
  backface-visibility: hidden;
  display: flex;
  flex-direction: column;
  min-height: 100vh;
  max-width: 100%;
  position: relative;
}
.v-responsive {
  position: relative;
  overflow: hidden;
  flex: 1 0 auto;
  max-width: 100%;
  display: flex;
}
.primary-text {
  color: #5100d1;
  caret-color: #5100d1;
}
.text {
  font-family: Arial, Helvetica, sans-serif;
  color: gray;
}

.nav {
  display: flex;
  height: 80px;
  margin-top: 0px;
  left: 0px;
  right: 0px;
}

.home img {
  margin-left: -70px;
}

.content {
  margin-right: -130px;
}

.v-btn__content {
  color: gray;
}
</style>
