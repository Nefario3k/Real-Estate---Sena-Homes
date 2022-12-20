<template>
  <div class="">
    <!-- min-width="352" -->
    <v-card class="mx-auto my-12" max-width="352" style="border-radius: 0">
      <nuxt-link to="/property">
        <v-img
          height="250"
          lazy-src=./images/pngs/broken-image.png"
          :src="property.imgUrl"
          transition="slide-x-transition"
          :gradient="`rgba(32, 29, 29, 0.5), rgba(32, 29, 29, 0.15)`"
        ></v-img>
        <!-- <div
          class="cardIMg"
          :style="`
            background-image: linear-gradient(rgba(32, 29, 29, 0.5) , rgba(32, 29, 29, 0.15)), url('${property.imgUrl}');`"
        ></div> -->
      </nuxt-link>

      <v-card-title class="card-title">
        <span style="line-height: 30px">{{ property.title }}</span>
        <span
          @click="activeIcon = !activeIcon"
          :class="{ active: activeIcon }"
          class="favorite-icon"
        >
          <!-- <img src=./images/pngs/icon_favorite.png" alt="" /> -->
          <svg
            width="47"
            height="48"
            viewBox="0 0 47 48"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <circle
              cx="23.4446"
              cy="23.9819"
              r="22.5426"
              stroke="#DEE2E6"
              stroke-width="0.980114"
            />
            <path
              d="M16.5355 26.3429L23.3498 32.7443C23.5845 32.9648 23.7019 33.075 23.8403 33.1022C23.9026 33.1144 23.9667 33.1144 24.029 33.1022C24.1674 33.075 24.2848 32.9648 24.5195 32.7443L31.3339 26.3429C33.2511 24.5418 33.484 21.578 31.8714 19.4996L31.5682 19.1088C29.6392 16.6225 25.7671 17.0395 24.4116 19.8795C24.2202 20.2807 23.6491 20.2807 23.4577 19.8795C22.1022 17.0395 18.2301 16.6225 16.3011 19.1088L15.9979 19.4996C14.3854 21.578 14.6182 24.5418 16.5355 26.3429Z"
              stroke="#6D7175"
              stroke-width="0.980114"
            />
          </svg>
        </span>
      </v-card-title>

      <v-card-text class="card-text">
        <div class="property-price">2,100,000 AED</div>

        <div class="property-description">
          <p>Bella Casa, Dubai, Serena</p>
        </div>
      </v-card-text>

      <v-divider class="mx-4"></v-divider>

      <v-card-actions class="card-actions">
        <div class="action-wrapper">
          <span class="action-icon-container"
            ><img src=./images/pngs/icon_bed.png" alt=""
          /></span>
          <span>3 beds</span>
        </div>
        <div class="action-wrapper">
          <span class="action-icon-container"
            ><img src=./images/pngs/icon_bath.png" alt=""
          /></span>
          <span>4 baths</span>
        </div>
        <div class="action-wrapper">
          <span class="action-icon-container"
            ><img src=./images/pngs/icon_sqft.png" alt=""
          /></span>
          <span>2,850 sqft</span>
        </div>
      </v-card-actions>
      <span class="property-type" style="">{{ property.type }}</span>
    </v-card>
  </div>
</template>
<script>
export default {
  props: ["property"],
  data: () => ({
    activeIcon: false,
  }),

  methods: {},
  mounted() {},
};
</script>
<style lang="scss" scoped>
.v-card {
  border: 1px solid rgba(196, 194, 194, 0.61);
  font-family: "Epilogue";

  .property-type {
    position: absolute;
    top: 1rem;
    left: 1rem;
    padding: 0.5rem 2rem;
    background-color: #976f40;
    color: white;
    font-size: 0.98rem;
  }
}

.card-title {
  font-size: 2rem;
  font-weight: bolder;
  // margin-bottom: 2rem;
  height: 9.5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: nowrap;
  white-space: pre-wrap;
  word-break: break-word;

  .favorite-icon {
    width: 4.7rem;
    height: 4.7rem;
    border-radius: 50%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    cursor: pointer;
  }

  .favorite-icon.active svg path {
    fill: var(--primary-color);
    stroke: var(--primary-color);
    transition: all 0.3s linear;
  }

  .favorite-icon.active svg circle {
    stroke: var(--primary-color);
    transition: all 0.2s linear;
  }
}

.v-card__text {
  padding-bottom: 0rem;
}

.card-text {
  .property-price {
    font-size: 2rem;
    color: #bf9001;
    margin-bottom: 3rem;
    font-weight: 700;
  }

  .property-description {
    font-size: 1.6rem;
    color: #808494;
  }
}

.card-actions {
  justify-content: space-between;
  padding: 20px 10px 20px 0;

  div {
    // border: 1px solid gray;
    flex-grow: 1;
    text-align: center;
    font-size: 1.2rem;
  }

  .action-wrapper {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 5px;

    .action-icon-container {
      width: 3.5rem;
      height: 3.5rem;
      background-color: #dee2e6;
      border-radius: 50%;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .action-wrapper {
      display: flex;
      align-items: center;
      justify-content: center;

      .action-icon-container {
        width: 3rem;
        height: 3rem;
        background-color: #dee2e6;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;

        img {
        }
      }

      span {
        margin-left: 0.5rem;
      }
    }

    .v-btn--icon.v-size--small .v-icon,
    .v-btn--fab.v-size--small .v-icon {
      color: red !important;
    }
  }
}

.v-card {
  border: none !important;
  box-shadow: none !important;
  filter: drop-shadow(0px 4.46px 8px rgba(28, 33, 43, 0.09));
}
.cardIMg {
  height: 250px;
  width: 100%;
  // background: linear-gradient(
  //     93deg,
  //     rgba(28, 33, 43, 0.7) 0%,
  //     rgba(28, 33, 43, 0.7) 20%
  //   ),
  //   url(./images/pngs/hero-img.png");
  background-size: cover;
}
</style>