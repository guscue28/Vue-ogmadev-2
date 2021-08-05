<template>
  <div id="footer">
    <b-container class="bv-example-row">
      <b-row>
        <b-col>
          <h5>2018 - 2021 <strong>Ogma</strong></h5></b-col
        >
        <b-col></b-col>
        <b-col>
          <a
            href="https://www.facebook.com/Ogma-Development-105175747920043/?ref=page_internal"
            class="btn"
            target="blank"
            ><strong>FACEBOOK</strong></a
          >
          <a
            href="https://www.instagram.com/ogma.studio/"
            class="btn"
            target="blank"
            ><strong>INSTAGRAM</strong></a
          >
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
#footer {
  height: 34px;
  background: rgba(226, 226, 226, 0.911);
  display: flex;
  flex-direction: column;
}
h5 {
  font-size: 13px;
}
a {
  font-size: 13px;
}
a:hover {
  background: rgb(160, 160, 160);
}
</style>
