<template>
  <div v-b-hover="hoverHandler" class="header">
    <b-row id="row">
      <b-col :cols="isHovered ? '8' : '12'" id="col">
        <div class="cont">
          <br /><br /><br /><br />
          <div
            class="mt-5 primary-text"
            style="display: flex; justify-content: center; font-size: 40px"
          >
            Web Development
            <br />
            & Mobile App solutions
          </div>
          <div
            class="text"
            style="display: flex; justify-content: center; font-size: 25px"
          >
            Technology Solutions Agency for
            <br />
            Websites, Web Systems, E-commerce
            <br />
            & Mobile Applications
          </div>
        </div>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      isHovered: false,
    };
  },
  methods: {
    hoverHandler(isHovered) {
      this.isHovered = isHovered;
    },
  },
};
</script>

<style>
.header {
  height: 500px;
  width: 100%;
  margin-top: 20px;
  display: flex;
  flex-direction: column;
}
.cont {
  width: 100%;
}
#row {
  height: 100%;
  background-image: url("https://ogma.dev/_nuxt/img/Banner-principal.9ec8154.png");
  background-position: right center;
  background-size: contain;
  background-repeat: no-repeat;
}
#col {
  background: white;
  box-shadow: 0 0 6px white;
}
</style>
