<template>
  <v-dialog
    v-model="showModal"
    :fullscreen="fullScreenModal"
    origin="center center"
    width="460"
    class="authDialog"
  >
    <v-card class="authCard" :class="{ fullscreen: fullScreenModal }">
      <div class="closeNavBtn" :class="{ hidden: !fullScreenModal }">
        <svg
          @click="showModal = false"
          width="30"
          height="31"
          viewBox="0 0 30 31"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect y="0.974609" width="30" height="29.9625" fill="#BF9001" />
          <path
            d="M11.25 12.2109L18.75 19.7016"
            stroke="white"
            stroke-linecap="round"
          />
          <path
            d="M18.75 12.2109L11.25 19.7016"
            stroke="white"
            stroke-linecap="round"
          />
        </svg>
      </div>
      <div class="modal_content">
        <form class="content_area">
          <header>Get started in minutes</header>
          <v-row class="row_form">
            <div class="col-12">
              <label for="fname">First Name</label>
              <input id="fname" type="text" name="" value="" />
            </div>
            <div class="col-12">
              <label for="lname">Last Name</label>
              <input id="lname" type="text" name="" value="" />
            </div>
            <div class="col-12">
              <label for="email">Email</label>
              <input id="email" type="email" name="" value="" />
            </div>
            <div class="col-12">
              <label for="phone">Phone Number</label>
              <input id="phone" type="text" name="" value="" />
            </div>
            <div class="col-12">
              <label for="password">Password</label>
              <input id="password" type="password" name="" value="" />
            </div>
            <div class="col-12">
              <label for="cPassword">Confrim Password</label>
              <input id="cPassword" type="password" name="" value="" />
            </div>
          </v-row>
          <footer class="footer pb-5">
            <v-btn @click="register()" class="Btn">Register</v-btn>
            <p class="subtext">
              By coninuning, you agree to Sena Homes’s
              <nuxt-link to="">Terms and Conditions</nuxt-link> &
              <nuxt-link to="">Privacy Policy</nuxt-link>
            </p>
          </footer>
        </form>
      </div>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  data() {
    return {
      showModal: false,
      fullScreenModal: false,
    };
  },
  mounted() {
    var nx = window.innerWidth;
    if (nx <= 959) {
      this.fullScreenModal = true;
    }
    window.addEventListener("resize", function (event) {
      var w = window.innerWidth;
      nx = w;
    });
    $(window).resize(() => {
      if (nx <= 959) {
        this.fullScreenModal = true;
      } else {
        this.fullScreenModal = false;
      }
    });
  },
  methods: {
    showAuthModal() {
      this.showModal = true;
    },
    register() {
      this.$emit("userLoggedIn");
      this.showModal = false;
    },
  },
};
</script>

<style scoped>
.modal_content {
  overflow: auto !important;
  height: 90vh !important;
}
.fullscreen {
  height: 100vh !important;
}
::-webkit-scrollbar {
  width: 10px !important;
  height: 10px !important;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: none;
  border-radius: 10px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: var(--primary-color);
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: var(--primary-color);
  transition: all 0.5s linear;
}
</style>