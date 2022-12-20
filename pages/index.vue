<template>
  <div id="home">
    <section id="heroSection" class="">
      <!-- bg slider  -->
      <ul class="heroSlideshow">
        <li><span>Image</span></li>
        <li><span>Image</span></li>
        <li><span>Image</span></li>
      </ul>
      <v-container class="hero_container">
        <header>Easy way to find a Perfect property.</header>
        <p class="subtext">
          A great platform to rent, lease, or even buy properties without any
          commissions.
        </p>
        <div class="search_wrapper">
          <v-row class="search_row">
            <div class="col-12 col-sm-3 col-md-3 col-lg-3 col-xl-3">
              <!-- buy  -->
              <v-menu
                allow-overflow
                :nudge-bottom="nudge_bottom"
                bottom
                offset-y
                :max-height="204"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown">
                    <span class="dropActive">Buy</span>
                    <svg
                      width="10"
                      height="6"
                      viewBox="0 0 10 6"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M4.80794 5.76953L1.09346 1.31215C0.659238 0.791085 1.02976 -4.31825e-07 1.70803 -4.02177e-07L8.29197 -1.14384e-07C8.97024 -8.47357e-08 9.34076 0.791085 8.90654 1.31215L5.19206 5.76953C5.09211 5.88947 4.90789 5.88947 4.80794 5.76953Z"
                        fill="#1C212B"
                      />
                    </svg>
                  </div>
                </template>
                <v-list class="searchList featured">
                  <v-list-item>
                    <v-list-item-title>Sale</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Rent</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Shortlet</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Lease</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Sale</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Rent</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Shortlet</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Lease</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-menu>
            </div>
            <div class="col-12 col-sm-3 col-md-3 col-lg-3 col-xl-3">
              <v-menu allow-overflow :nudge-bottom="nudge_bottom" offset-y>
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown">
                    <span>Emirate</span>
                    <svg
                      width="10"
                      height="6"
                      viewBox="0 0 10 6"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M4.80794 5.76953L1.09346 1.31215C0.659238 0.791085 1.02976 -4.31825e-07 1.70803 -4.02177e-07L8.29197 -1.14384e-07C8.97024 -8.47357e-08 9.34076 0.791085 8.90654 1.31215L5.19206 5.76953C5.09211 5.88947 4.90789 5.88947 4.80794 5.76953Z"
                        fill="#1C212B"
                      />
                    </svg>
                  </div>
                </template>
                <v-list class="searchList">
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-menu>
            </div>
            <div class="col-12 col-sm-3 col-md-3 col-lg-3 col-xl-3">
              <v-menu allow-overflow offset-y :nudge-bottom="nudge_bottom">
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown">
                    <span>City</span>
                    <svg
                      width="10"
                      height="6"
                      viewBox="0 0 10 6"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M4.80794 5.76953L1.09346 1.31215C0.659238 0.791085 1.02976 -4.31825e-07 1.70803 -4.02177e-07L8.29197 -1.14384e-07C8.97024 -8.47357e-08 9.34076 0.791085 8.90654 1.31215L5.19206 5.76953C5.09211 5.88947 4.90789 5.88947 4.80794 5.76953Z"
                        fill="#1C212B"
                      />
                    </svg>
                  </div>
                </template>
                <v-list class="searchList">
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-menu>
            </div>
            <div class="col-12 col-sm-3 col-md-3 col-lg-3 col-xl-3">
              <v-btn class="Btn">Search</v-btn>
            </div>
          </v-row>
        </div>
      </v-container>
    </section>
    <section id="property_carousel_section">
      <v-container>
        <property-list
          title="Buying a property"
          :properties="properties"
        ></property-list>
        <property-list
          title="Renting a property"
          :properties="properties"
        ></property-list>
        <property-list
          title="Off-plan Properties"
          :properties="properties"
        ></property-list>
      </v-container>
    </section>
    <FindComfortRE />
    <FindBestRE />
    <FAQ />
    <MobileApp />
  </div>
</template>

<script>
export default {
  data() {
    return {
      nudge_bottom: 10,
      properties: [
        {
          title: "Serena with a very long name for the property",
          imgUrl:
            "https://images.unsplash.com/photo-1600585153490-76fb20a32601?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80",
          description: "Bella Casa, Dubai, Serena",
          price: 2100000,
          type: "Villa",
        },
        {
          title: "AL Quoz 4",
          imgUrl:
            "https://images.unsplash.com/photo-1600047509782-20d39509f26d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=701&q=80",
          description: "Bella Casa, Dubai, Serena",
          price: 2100000,
          type: "Villa",
        },
        {
          title: "Imperial Avenue",
          imgUrl:
            "https://images.unsplash.com/photo-1600607688969-a5bfcd646154?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80",
          description: "Bella Casa, Dubai, Serena",
          price: 2100000,
          type: "Apartment",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
/* pages animation  */

#home {
  /* animation: transIn 0.8s linear 0s; */
  overflow: hidden;
}

@keyframes transIn {
  from {
    opacity: 0;
    transform: translateX(5px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

#heroSection {
  min-height: 100vh;
  width: 100vw;
  margin-top: -96px;
}

.heroSlideshow,
.heroSlideshow:after {
  position: absolute;
  width: 100%;
  height: 100vh;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 0;
  margin-top: -96px;
  background: linear-gradient(
    93deg,
    rgba(28, 33, 43, 0.7) 0%,
    rgba(28, 33, 43, 0.7) 20%
  );
  overflow: hidden !important;
}

.heroSlideshow li {
  list-style-type: none;
}

.heroSlideshow:after {
  display: none;
  content: "";
  background: linear-gradient(
    93deg,
    rgba(28, 33, 43, 0.7) 0%,
    rgba(28, 33, 43, 0.7) 20%
  );
}

.heroSlideshow li span {
  width: 100%;
  height: 100%;
  margin-top: -2.4%;
  position: absolute;
  top: 0;
  left: 0;
  color: transparent;
  background-position: 100%;
  background-repeat: no-repeat;
  opacity: 0;
  z-index: 0;
  /* transform: scale(0.8); */
  animation: slideshow 12s linear infinite 0s;
}

.heroSlideshow li:nth-child(1) span {
  background: linear-gradient(
      93deg,
      rgba(28, 33, 43, 0.7) 0%,
      rgba(28, 33, 43, 0.7) 20%
    ),
    url(./images/pngs/hero-img.png");
  background-size: cover;
  background-position: 100%;
}

.heroSlideshow li:nth-child(2) span {
  background: linear-gradient(
      93deg,
      rgba(28, 33, 43, 0.7) 0%,
      rgba(28, 33, 43, 0.7) 20%
    ),
    url(./images/pngs/hero-img-2.png");
  background-size: cover;
  animation-delay: 4s;
}

.heroSlideshow li:nth-child(3) span {
  background: linear-gradient(
      93deg,
      rgba(28, 33, 43, 0.7) 0%,
      rgba(28, 33, 43, 0.7) 20%
    ),
    url(./images/pngs/hero-img-3.png");
  background-size: cover;
  animation-delay: 8s;
}

@keyframes slideshow {
  0% {
    opacity: 0;
    animation-timing-function: ease-in;
  }

  8% {
    opacity: 1;
    transform: scale(1.05);
    animation-timing-function: ease-out;
  }

  17% {
    opacity: 1;
    transform: scale(1.1);
  }

  25% {
    opacity: 1;
    transform: scale(1.1);
  }

  50% {
    opacity: 0;
    transform: scale(1.1);
  }

  100% {
    opacity: 0;
  }
}

.hero_container {
  display: flex;
  /* display: none; */
  position: relative;
  z-index: 3;
  justify-content: center;
  height: 100%;
  min-height: 100vh;
  flex-direction: column;
}

.hero_container header {
  font-weight: 700;
  font-size: 6rem;
  color: #fff;
  width: 50%;
  margin-top: 117px;
  margin-bottom: 20px;
  line-height: 66px;
}

.hero_container p.subtext {
  font-weight: 400;
  font-size: 2.4rem;
  color: #fff;
  width: 50%;
}

.search_wrapper {
  min-height: 13.3rem;
  background: rgba(255, 255, 255, 0.6);
  box-shadow: 0px 30px 60px -15px rgba(143, 144, 188, 0.15);
  backdrop-filter: blur(10px);
  display: flex;
  align-items: center;
  padding: 30px 0;
  margin-top: 40px;
}

.search_row {
  margin-left: 5%;
  margin-right: 5%;
}

.dropdown {
  display: flex;
  align-items: center;
  justify-content: space-between;
  border: 1px solid rgba(191, 144, 1, 0.21);
  box-shadow: 0px 30px 60px -15px rgba(143, 144, 188, 0.15);
  backdrop-filter: blur(10px);
  background-color: #fff;
  min-height: 4.9rem;
  padding: 0 15px;
}

.dropdown span {
  color: var(--faded-color);
  font-weight: 500;
  font-size: 1.8rem;
}

.dropdown span.dropActive {
  color: var(--secondary-color);
}

.Btn {
  width: 100%;
  min-height: 4.9rem;
  font-weight: 700;
  font-size: 1.2rem;
  border-radius: 0;
  box-shadow: none;
  background: var(--primary-color) !important;
  color: #fff;
  border: 1px solid var(--primary-color);
}

#property_carousel_section {
  background-image: url(/images/svg/geometry01.svg),
    url(/images/svg/geometry02.svg);
  background-position: top right, bottom left;
  background-repeat: no-repeat;
  background-size: 25%;
}
.searchList {
  padding-top: 28px;
  .bedTitle {
    min-height: auto;
    p {
      margin: 0;
      font-weight: 700;
      font-size: 1.6rem;
      color: var(--primary-color);
    }
  }
  .dropdown {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border: 1px solid rgba(191, 144, 1, 0.21);
    box-shadow: 0px 30px 60px -15px rgba(143, 144, 188, 0.15);
    backdrop-filter: blur(10px);
    background-color: #fff;
    min-height: 4.9rem;
    padding: 0 15px;
    margin-top: 12px;
  }

  .dropdown span {
    color: var(--faded-color);
    font-weight: 500;
    font-size: 1.8rem;
  }

  .dropdown span.dropActive {
    color: var(--faded-color);
  }
  .gridMenu {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    column-gap: 18px;
    row-gap: 9px;
    padding: 16px;
    margin-top: 28px;
    .gridItem {
      padding: 0;
      justify-content: center;
      height: 3rem;
      min-height: 3rem;
      border: 1px solid var(--border05-color);
      font-weight: 500;
      font-size: 1.2rem;
      color: var(--label02-color);
      cursor: pointer;
      &:hover {
        color: var(--primary-color);
        border: 1px solid var(--primaryLte-color);
        background-color: var(--hover-gradient-bg);
      }
    }
  }
  .Btn {
    width: 100%;
    min-height: 4.9rem;
    font-weight: 700;
    font-size: 1.8rem;
    border-radius: 0;
    box-shadow: none;
    background: var(--primary-color) !important;
    color: #fff;
    border: 1px solid var(--primary-color);
    grid-column: span 2;
    text-transform: none;
    p {
      margin: 0;
      font-size: 1.8rem;
    }
  }
  .Btn.reset {
    background: transparent !important;
    color: var(--primary-color);
    border: 1px solid var(--primaryLte-color);
    p {
      color: var(--faded02-color);
    }
  }
}
.v-menu__content.theme--light.menuable__content__active:has(.searchList) {
  border-radius: 0;
}
.searchList.featured {
  padding-top: 18px;
  .v-list-item {
    justify-content: center;
    margin: 0 10px;
    cursor: pointer;
    &:hover {
      background-color: var(--hover-gradient-bg);
      .v-list-item__title {
        color: var(--primary-color);
      }
    }
    .v-list-item__title {
      flex: none;
      color: var(--faded-color);
      font-size: 1.4rem;
      font-weight: 500;
    }
  }
}
::-webkit-scrollbar {
  width: 5px !important;
  height: 5px !important;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: none;
  background: var(--faded-color);
  /* border-radius: 10px; */
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: var(--primary-color);
  // border-radius: 10px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: var(--primary-color);
  transition: all 0.5s linear;
}
@media (max-width: 768px) {
  #property_carousel_section {
    background-color: #fcfcfc;
    background-size: 75% !important;
  }
}
</style>
