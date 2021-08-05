<template>
  <div id="low">
    <b-container>
      <b-row style="display: flex;">
        <b-col cols="6">
          <form action="">
            <div class="form">
              <h1 id="title" class="mt-5 primary-text">Contact Us</h1>
              <p class="text izq">
                Our mission is to make your business grow through digital
                solutions which allow you to gain a competitive advantage. Write
                us!
              </p>
              <div class="mb-3">
                <br />

                <input
                  type="text"
                  class="form-control"
                  id="name"
                  placeholder="Full Name"
                  v-model="datosPersona.name"
                />
                <span v-if="!datosPersona.name" class="required"
                  >Full Name is required</span
                >
              </div>
              <div class="mb-3">
                <input
                  type="email"
                  class="form-control"
                  id="email"
                  placeholder="Email"
                  v-model="datosPersona.email"
                />
                <span v-if="!datosPersona.email" class="required"
                  >Email is required</span
                >
                <span class="required" v-if="stop">Invalid email</span>
              </div>
              <div class="mb-3">
                <textarea
                  id="mensaje"
                  cols="42"
                  rows="5"
                  placeholder="Write your message her"
                  v-model="datosPersona.mensaje"
                ></textarea
                ><br />
                <span v-if="!datosPersona.mensaje" class="required"
                  >Mensage is required</span
                >
              </div>
              <b-row>
                <b-col></b-col>
                <b-col>
                  <div
                    class="mb-3"
                    style="display:flex;   justify-content: right;"
                  >
                    <button
                      class="btn"
                      :disabled="btnDisabled"
                      style=" width: 160px; height: 35px; border-radius: 15px; background: #5100d1; color: white;"
                      @click.prevent="enviar"
                    >
                      Send
                    </button>
                  </div>
                </b-col>
              </b-row>
            </div>
          </form>
        </b-col>
        <b-col cols="6">
          <div class="img1" style=" ">
            <img
              id="img"
              src="	https://ogma.dev/_nuxt/img/contact-avatar.4a56327.png"
              alt="fondo"
              width="400px"
              height="400px"
            />
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import axios from "vue-axios";
export default {
  name: "Low",
  data() {
    return {
      datosPersona: {
        name: "",
        email: "",
        mensaje: "",
      },

      enviado: true,
      stop: "",
      validation: true,
    };
  },
  methods: {
    async enviar() {
      var payload = JSON.stringify(this.datosPersona);
      console.log(payload);
      this.enviado = true;
      await axios.post("/project", payload).then((res) => {
        console.log(res);
      });
    },
    validar() {
      var arroba = this.datosPersona.email.indexOf("@");
      var punto = this.datosPersona.email.indexOf(".");
      if (arroba == -1 || punto == -1) {
        this.stop = true;
      } else {
        this.stop = false;
      }
    },
  },
  computed: {
    btnDisabled() {
      const vm = this;
      if (
        vm.datosPersona.name.length === 0 ||
        vm.datosPersona.email.length === 0 ||
        vm.datosPersona.mensaje.length === 0
      ) {
        return true;
      } else {
        return false;
      }
    },
  },
};
</script>

<style>
.form {
  width: 400px;
  margin-left: 50px;
}
.required {
  color: red;
}
.izq {
  text-align: left;
}
.btn:disabled {
  background: rgba(255, 255, 255, 0.5);
}

.img1 {
  display: flex;
  justify-content: center;
  margin-right: -200px;
}
</style>
