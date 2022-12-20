<template>
  <div>
    <v-navigation-drawer
      app
      v-model="drawer"
      color="var(--secondary-color)"
      temporary
      right
    >
      <div class="closeNavBtn">
        <svg
          @click="drawer = false"
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
      <v-list nav dense>
        <v-list-item-group v-model="group">
          <nuxt-link to="/property/residential">
            <v-list-item class="navList">
              <v-list-item-title class="navListItem"
                >Residential</v-list-item-title
              >
            </v-list-item>
          </nuxt-link>
          <nuxt-link to="/property/commercial">
            <v-list-item class="navList">
              <v-list-item-title class="navListItem"
                >Commercial</v-list-item-title
              >
            </v-list-item>
          </nuxt-link>
          <nuxt-link to="/property/off-plan">
            <v-list-item class="navList">
              <v-list-item-title class="navListItem"
                >Off-plan Projects</v-list-item-title
              >
            </v-list-item>
          </nuxt-link>
          <nuxt-link to="/about">
            <v-list-item class="navList">
              <v-list-item-title class="navListItem"
                >About Us</v-list-item-title
              >
            </v-list-item>
          </nuxt-link>
          <nuxt-link to="/contact-us">
            <v-list-item class="navList">
              <v-list-item-title class="navListItem"
                >Contact Us</v-list-item-title
              >
            </v-list-item>
          </nuxt-link>
        </v-list-item-group>
      </v-list>
      <div v-if="!loggedIn" class="bottomNav">
        <v-btn @click="showModal('login')" class="Btn">Login</v-btn>
        <v-btn @click="showModal('register')" class="registerBtn Btn"
          >Register</v-btn
        >
      </div>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  props: ["loggedIn"],
  data() {
    return {
      drawer: false,
      group: null,
    };
  },
  methods: {
    showNavBar() {
      this.drawer = true;
    },
    showModal(type) {
      this.drawer = false;
      this.$emit("showMobileModal", type);
    },
  },
};
</script>

<style scoped>
.bottomNav {
  position: absolute;
  bottom: 5%;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  gap: 20px;
}
.Btn {
  width: 10.6rem;
  height: 4.8rem;
  font-weight: 700;
  font-size: 1.2rem;
  border-radius: 0;
  box-shadow: none;
  background: transparent !important;
  color: var(--primary-color);
  border: 1px solid var(--primary-color);
}
.registerBtn.Btn {
  background: var(--primary-color) !important;
  color: #fff;
  border: 1px solid var(--primary-color);
}
</style>