<template>
  <div id="top">
    <b-row id="T-hig">
      <b-col cols="6">
        <b-row>
          <img
            id="life"
            src="https://ogma.dev/_nuxt/img/Banner-aboutUs.84bcf44.png"
            alt="imagen"
            width="600"
            height="600"
          />
        </b-row>
      </b-col>
      <b-col cols="6">
        <br /><br /><br /><br /><br />
        <h2 class="primary-text text-center">About</h2>
        <h5 class="text text-center">
          We are a company with a team of professionals and specialists in
          developing systems, applications, websites & digital marketing. Our
          team work is oriented to create functional products, totally adapted
          to the client's needs.
        </h5>
      </b-col>
    </b-row>
    <b-row id="T-mid" class="text-center">
      <b-col cols="12">
        <div class="banner-parallax">
          <!--<h1>Speed and quality</h1>
          <br /><br />
          <h1>are our reality at Ogma</h1>-->
          Speed and quality
          <br />
          are our reality at Ogma
        </div>
      </b-col>
    </b-row>
    <b-row>
      <b-col class="text-center">
        <img
          id="fondo"
          src="https://ogma.dev/_nuxt/img/Danfra.6f4a7e2.jpg"
          alt="imagen2"
        />
      </b-col>
      <b-col>
        <br /><br /><br /><br /><br />
        <h5 class="text" style="text-align: justify;">
          We work with technology to drive constant growth and create a digital
          base that allows expanding the reach of our clients & profitability of
          their business
        </h5>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: "Top",
};
</script>

<style>
#top {
  width: 100%;
  max-width: 100%;
  display: flex;
  flex-wrap: wrap;
}
#life {
  width: 100%;
  height: 100%;
}
.banner-parallax {
  width: 100%;
  height: 450px;
  background: url("https://ogma.dev/_nuxt/img/Banner-Quality.c86f29b.png");
  background-repeat: no-repeat;
  background-position: cover;
  background-attachment: fixed;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-family: sans-serif;
  font-size: 65px;
}

#fondo {
  width: 100%;
  height: 100%;
}
</style>
