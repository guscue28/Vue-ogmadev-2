<template>
  <div id="middle2" class="mid2" v-b-hover="hoverHandler">
    <div class="fondo1">
      <b-row
        :style="
          isHovered
            ? 'background: rgba(255,255,255,0.5); height: 450px'
            : 'height: 450px'
        "
      >
        <b-col
          class="logo"
          :style="
            isHovered
              ? 'background-image: url(&quot;data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyOTkuNDIzIiBoZWlnaHQ9IjI1OS4yNSIgdmlld0JveD0iMCAwIDI5OS40MjMgMjU5LjI1Ij4NCiAgPGcgaWQ9Ikljb24iIHRyYW5zZm9ybT0idHJhbnNsYXRlKC00MTAuNTkgLTYwNC40MTcpIj4NCiAgICA8cGF0aCBpZD0iVHJhemFkb183IiBkYXRhLW5hbWU9IlRyYXphZG8gNyIgZD0iTTUwNS41NTIsNzM4LjVsMzcuMzc1LDQyLjU2NmExNi45NzksMTYuOTc5LDAsMCwwLDI0LjUwOSwxLjA1M0w3MjIuMyw2MzMuNjUyYTE2Ljk3OSwxNi45NzksMCwwLDAtMjMuNS0yNC41MTNMNTU2LjczOSw3NDUuMzI5LDUzMS4wNyw3MTYuMDkzYTE2Ljk3OSwxNi45NzksMCwwLDAtMjUuNTE4LDIyLjRaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTcuNTE0KSIgZmlsbD0iIzUxMDBkMSIvPg0KICAgIDxwYXRoIGlkPSJUcmF6YWRvXzgiIGRhdGEtbmFtZT0iVHJhemFkbyA4IiBkPSJNNjE4LjEzNSw3NDcuOTY2YTgxLjc4OCw4MS43ODgsMCwxLDEtMzIuODUzLTc0LjkyOUw2MTcuODcsNjQxLjhhMTI2LjE5MiwxMjYuMTkyLDAsMSwwLDQxLjcxNyw2Ni40MzFaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwIC0xLjU1MykiIGZpbGw9IiM1MTAwZDEiLz4NCiAgPC9nPg0KPC9zdmc+DQo=&quot;); background-position: center center;'
              : ''
          "
        >
        </b-col>
        <b-col id="contenido">
          <br /><br />
          <div
            class="first"
            :style="isHovered ? 'color: #5100d1;' : 'color: white;'"
          >
            Do you still think is
            <br />
            not posible ?
          </div>
          <div
            class="second"
            :style="isHovered ? 'color: gray;' : 'color: white;'"
          >
            Have your own ecommerce quickly & easy.
            <br />
            Ecommerce is one of the sales methods with the highest annual
            growth, start now!
          </div>
          <br />
          <button
            class="btn btn-block"
            id="button"
            v-scroll-to="{ el: '#vlow', offset: -60 }"
          >
            START NOW
          </button>
        </b-col>
        <b-col class="logo-container">
          <br /><br />
          <transition name="image-fade">
            <img
              src="https://ogma.dev/_nuxt/img/Macbook-e-commerce.cfb23ef.png"
              :class="isHovered ? 'enter' : 'leave'"
              width="550px"
              height="80%"
              class="mt-12 image-logo"
            />
          </transition>
        </b-col>
      </b-row>
    </div>
  </div>
</template>

<script>
export default {
  name: "Middle2",
  data() {
    return {
      isHovered: false,
      show: true,
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
.mid2 {
  display: flex;
  flex-direction: column;
  height: auto;
  width: 100%;
  background: url("https://ogma.dev/_nuxt/img/Banner-e-commerce.f82def1.png");
  background-position: center center;
  background-size: cover;
}

.logo {
  margin-left: -150px;
  background-image: url("data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyOTkuNDIzIiBoZWlnaHQ9IjI1OS4yNSIgdmlld0JveD0iMCAwIDI5OS40MjMgMjU5LjI1Ij4NCiAgPGcgaWQ9Ikljb24iIHRyYW5zZm9ybT0idHJhbnNsYXRlKC00MTAuNTkgLTYwNC40MTcpIj4NCiAgICA8cGF0aCBpZD0iVHJhemFkb183IiBkYXRhLW5hbWU9IlRyYXphZG8gNyIgZD0iTTUwNS41NTIsNzM4LjVsMzcuMzc1LDQyLjU2NmExNi45NzksMTYuOTc5LDAsMCwwLDI0LjUwOSwxLjA1M0w3MjIuMyw2MzMuNjUyYTE2Ljk3OSwxNi45NzksMCwwLDAtMjMuNS0yNC41MTNMNTU2LjczOSw3NDUuMzI5LDUzMS4wNyw3MTYuMDkzYTE2Ljk3OSwxNi45NzksMCwwLDAtMjUuNTE4LDIyLjRaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTcuNTE0KSIgZmlsbD0iI2ZmZiIvPg0KICAgIDxwYXRoIGlkPSJUcmF6YWRvXzgiIGRhdGEtbmFtZT0iVHJhemFkbyA4IiBkPSJNNjE4LjEzNSw3NDcuOTY2YTgxLjc4OCw4MS43ODgsMCwxLDEtMzIuODUzLTc0LjkyOUw2MTcuODcsNjQxLjhhMTI2LjE5MiwxMjYuMTkyLDAsMSwwLDQxLjcxNyw2Ni40MzFaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwIC0xLjU1MykiIGZpbGw9IiNmZmYiLz4NCiAgPC9nPg0KPC9zdmc+DQo=");
  background-position: center center;
  background-size: auto;
  background-repeat: no-repeat;
}

.first {
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  color: white;
  font-family: sans-serif;
  font-size: 40px;
}

.second {
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  color: white;
  font-family: sans-serif;
  font-size: 20px;
}
#button {
  background: white;
  color: #5100d1;
  caret-color: #5100d1;
  text-align: center;
  display: block;
  height: 35px;
  width: 145px;
  border-radius: 15px;
}

.image-logo {
  transition: all ease-in-out 0.3s;
}

.image-logo.enter {
  transform: scale(1);
}

.image-logo.leave {
  transform: scale(0);
}

/*.fondo1:hover {
  background: rgba(235, 236, 236, 0.88);
}*/
</style>
