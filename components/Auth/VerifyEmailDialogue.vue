<template>
  <v-dialog
    v-model="showModal"
    :fullscreen="fullScreenModal"
    origin="center center"
    width="460"
    class="authDialog"
  >
    <v-card class="authCard">
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
        <div class="content_area">
          <header style="margin-bottom: 11px">Forgot Password?</header>
          <p
            style="
              text-align: center;
              width: 85%;
              margin: 0 auto;
              color: #222;
              font-size: 1.4rem;
              font-weight: 400;
            "
          >
            Enter the 4-digit Code code sent to your email address
          </p>
          <v-row class="row_form">
            <div class="col-12">
              <v-otp-input
                plain
                length="4"
                v-model="token.val"
                type="number"
                required
                class="reg_otp_input"
                @finish="showResetPassword()"
              ></v-otp-input>
            </div>
          </v-row>
          <footer class="footer">
            <v-btn @click="showResetPassword()" class="Btn">Continue</v-btn>
          </footer>
        </div>
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
      token: {
        val: "",
      },
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
    showResetPassword() {
      this.$emit("showResetPassword");
      this.token.val = "";
      this.showModal = false;
    },
  },
};
</script>

<style scoped>
</style>