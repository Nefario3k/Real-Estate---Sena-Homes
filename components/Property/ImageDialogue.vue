<template>
  <v-dialog
    v-model="showModal"
    :fullscreen="true"
    origin="center center"
    width="460"
    class="imgViewDilogue"
  >
    <v-card
      class="imgCard"
      style="box-shadow: none; margin: 0; border-radius: 0"
    >
      <v-row style="margin: 0 !important">
        <div class="col-12 relative">
          <div class="img_header">
            <p class="goldText">Images</p>
          </div>
          <div class="closeNavBtn">
            <svg
              @click="showModal = false"
              width="40"
              height="40"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle cx="25" cy="25" r="25" fill="white" />
              <path
                d="M32.75 16.2498L16.25 32.7498"
                stroke="#BF9001"
                stroke-width="3"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M16.25 16.2498L32.75 32.7498"
                stroke="#BF9001"
                stroke-width="3"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
        <v-row class="modal_content col-12">
          <div class="col-2 control_wrapper">
            <svg
              v-if="tab > 0"
              @click="imgPreview('prev')"
              width="40"
              height="40"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle cx="25" cy="25" r="25" fill="white" />
              <path
                d="M20.375 24.5L19.3143 23.4393L18.2537 24.5L19.3143 25.5607L20.375 24.5ZM27.5643 15.1893L19.3143 23.4393L21.4357 25.5607L29.6857 17.3107L27.5643 15.1893ZM19.3143 25.5607L27.5643 33.8107L29.6857 31.6893L21.4357 23.4393L19.3143 25.5607Z"
                fill="#BF9001"
              />
            </svg>
          </div>
          <v-container
            class="img_large_container"
            :style="` background-image: url('${previewedImage}')`"
          >
          </v-container>
          <div class="col-2 control_wrapper right">
            <svg
              @click="imgPreview('next')"
              width="40"
              height="40"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle cx="25" cy="25" r="25" fill="white" />
              <path
                d="M28.625 24.5L29.6857 23.4393L30.7463 24.5L29.6857 25.5607L28.625 24.5ZM21.4357 15.1893L29.6857 23.4393L27.5643 25.5607L19.3143 17.3107L21.4357 15.1893ZM29.6857 25.5607L21.4357 33.8107L19.3143 31.6893L27.5643 23.4393L29.6857 25.5607Z"
                fill="#BF9001"
              />
            </svg>
          </div>
        </v-row>
      </v-row>

      <!-- option 0ne  -->
      <!-- <div class="media_scroller scrollSnap01">
        <div v-for="(items, index) in 9" :key="index" class="media_element">
          <img
            @click="preview(items)"
            loading="lazy"
            :src="`${media[0].src + items}.png`"
            alt=""
          />
        </div>
      </div> -->
      <!-- option two  -->
      <v-tabs
        centered
        fixed-tabs
        height="125"
        :show-arrows="false"
        slider-color="var(--primary-color)"
        :slider-size="3"
        background-color="transparent"
        center-active
        dark
        v-model="tab"
        class="scrollSnap01"
      >
        <v-tab
          :ripple="false"
          class="tab_img"
          v-for="(items, index) in 9"
          :key="index"
          @click="preview(items)"
        >
          <img
            loading="lazy"
            :src="`${media[0].src + items}.png`"
            alt=""
          /> </v-tab
      ></v-tabs>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  data() {
    return {
      showModal: false,
      tab: 0,
      previewedImage: null,
      media: [{ src: "/images/pngs/smallProp0" }],
    };
  },
  mounted() {
    this.previewedImage = "/images/pngs/largeProp.png";
  },
  methods: {
    showImgModal() {
      this.showModal = true;
    },
    showForgotPassword() {
      this.$emit("showForgotPassword");
      this.showModal = false;
    },
    imgPreview(type) {
      switch (type) {
        case "prev":
          if (this.tab === "" || this.tab === null || this.tab == 0) {
            return;
          } else {
            this.previewedImage = "/images/pngs/smallProp0" + this.tab + ".png";
            this.tab = this.tab - 1;
          }
          break;
        case "next":
          var next = this.tab + 2;
          this.tab = this.tab + 1;
          this.previewedImage = "/images/pngs/smallProp0" + next + ".png";

          break;

        default:
          break;
      }
    },
    preview(type) {
      this.previewedImage = "/images/pngs/smallProp0" + type + ".png";
    },
  },
};
</script>

<style lang="scss" scoped>
.img_header {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0px 21px 13px;
  p {
    padding: 0 30px 5px;
    border-bottom: 2px solid var(--primary-color);
    color: var(--primary-color);
    font-weight: 700;
    font-size: 1.8rem;
  }
}
.closeNavBtn {
  position: absolute;
  display: block;
  top: 15%;
  right: 3%;
  padding: 0;
  svg:hover {
    circle {
      fill: var(--primary-color);
      transition: all 0.2s linear;
    }
    path {
      stroke: #fff !important;
      transition: all 0.2s linear;
    }
  }
}
.modal_content {
  padding-top: 0;
  margin: 0;
  margin-top: -12px;
  .img_large_container {
    height: 65vh;
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
    width: 65%;
    margin: auto;
    opacity: 1;
    transition: background-image 0.5s linear;
  }
}
.slider_container {
  margin: 0 !important;
  overflow: visible !important;
}

.media_scroller {
  --spacer: 2.4rem;
  display: grid;
  grid-auto-flow: column;
  grid-auto-columns: 22%;
  gap: var(--spacer);
  overflow-x: auto;
  overscroll-behavior-inline: contain;

  .media_element {
    margin: 1.4rem 0 var(--spacer, 2.4rem);
    border-radius: 0;
    background-color: var(--border-color);
  }
  img {
    inline-size: 100%;
    aspect-ratio: 16 / 9;
    object-fit: cover;
    cursor: pointer;
    overflow: hidden;
  }
}
.scrollSnap01 {
  scroll-snap-type: inline mandatory;
  padding-inline: calc(var(--spacer) / 2) !important;
  scroll-padding-inline: var(--spacer, 2.4rem);
  overflow-x: auto;
  overscroll-behavior-inline: contain;
}
.scrollSnap01 div.tab_img.v-tab {
  scroll-snap-align: start !important;
}
.tab_img {
  width: 100%;
  height: 100%;
  margin: 0 6px !important;
  padding: 0;
  background: transparent !important;

  img {
    inline-size: 100%;
    aspect-ratio: 16 / 9;
    object-fit: cover;
    cursor: pointer;
    overflow: hidden;
  }
}
.tab_img::before {
  display: none !important;
}
::-webkit-scrollbar {
  width: 10px;
  height: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: none;
  border-radius: 10px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: var(--secondary-color);
  border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: var(--primary-color);
  transition: all 0.5s linear;
}
.control_wrapper {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  svg {
    cursor: pointer;
    transition: all 0.5s linear;
  }
  svg:hover {
    circle {
      fill: var(--primary-color);
      transition: all 0.2s linear;
    }
    path {
      fill: #fff !important;
      transition: all 0.2s linear;
    }
  }
}
.control_wrapper.right {
  justify-content: flex-start;
}
@media (max-width: 959px) {
  .control_wrapper {
    display: none;
  }
}
</style>