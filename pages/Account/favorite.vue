<template>
  <section id="account">
    <v-container class="account_container">
      <div class="account_top_flex">
        <AccountNav v-on:userLoggedOut="$emit('userLoggedOut')" />
        <v-row class="page_body">
          <div class="col-12">
            <header @click="reviews = !reviews">Favorites</header>
          </div>
          <v-card class="border" v-if="!reviews">
            <div class="noReviews">
              <svg
                width="129"
                height="129"
                viewBox="0 0 129 129"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M23.9224 74.7566L61.2927 109.862C62.58 111.071 63.2236 111.676 63.9825 111.825C64.3242 111.892 64.6758 111.892 65.0175 111.825C65.7764 111.676 66.42 111.071 67.7073 109.862L105.078 74.7566C115.592 64.8794 116.869 48.6255 108.026 37.2276L106.363 35.0845C95.784 21.4494 74.5493 23.7361 67.1158 39.3109C66.0658 41.5109 62.9342 41.5109 61.8842 39.3109C54.4507 23.7361 33.216 21.4494 22.637 35.0845L20.9743 37.2276C12.1311 48.6255 13.4079 64.8794 23.9224 74.7566Z"
                  stroke="#808494"
                  stroke-width="5.375"
                />
              </svg>

              <p class="noProp_review">
                You haven’t favorited any properties yet
              </p>
              <p class="subtext">
                Save the properties you like for easy access on any device
              </p>
              <div class="cp_wrapper">
                <v-btn class="Btns" type="submit">Browse Properties</v-btn>
              </div>
            </div>
          </v-card>
          <v-row v-else class="propRow">
            <div class="col-12 col-sm-6 col-md-6 col-lg-6 col-xl-6">
              <property-card :property="properties[2]"></property-card>
            </div>
            <div class="col-12 col-sm-6 col-md-6 col-lg-6 col-xl-6">
              <property-card :property="properties[1]"></property-card>
            </div>
            <div class="col-12 col-sm-6 col-md-6 col-lg-6 col-xl-6">
              <property-card :property="properties[2]"></property-card>
            </div>
            <div class="col-12 col-sm-6 col-md-6 col-lg-6 col-xl-6">
              <property-card :property="properties[0]"></property-card>
            </div>
            <div class="text-center col-12">
              <v-pagination
                color="var(--primary-color)"
                v-model="page"
                :length="10"
                :total-visible="5"
                circle
              ></v-pagination>
            </div>
          </v-row>
        </v-row>
      </div>
    </v-container>
  </section>
</template>

<script>
export default {
  layout: "property",
  data() {
    return {
      reviews: false,
      page: 1,
      properties: [
        {
          title: "Serena",
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

<style lang="scss" scoped>
#account {
  padding-top: 61px;
}
.page_body {
  animation: transIn 0.3s linear 0s;
}

@keyframes transIn {
  from {
    opacity: 0;
    transform: translateY(15px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.account_top_flex {
  display: flex;
  gap: 133px;
  margin-bottom: 207px;
  header {
    font-size: 2.4rem;
    color: var(--primary-color);
    font-weight: 600;
    margin-left: -12px;
  }
  .border {
    border: 1px solid var(--border03-color);
    padding: 47px 26px;
    width: 100%;
    border-radius: 0;
    box-shadow: none;
    margin-top: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    min-height: 52.8rem;
    svg {
      display: inline;
      margin-bottom: 37px;
    }
    p {
      font-weight: 500;
      color: var(--greeter-color);
      font-size: 2rem;
      margin: 0;
    }
    p.subtext {
      font-weight: 400;
    }
  }
  .cp_wrapper {
    display: flex;
    justify-content: center;
    margin-top: 50px;
    .Btns {
      width: 22.4rem;
      height: 5.1rem;
      font-weight: 700;
      font-size: 1.2rem;
      border-radius: 0;
      box-shadow: none;
      background: var(--primary-color) !important;
      color: #fff;
      border: 1px solid var(--primary-color);
      margin-bottom: 11px;
      text-transform: capitalize;
    }
  }
}
@media (min-width: 1090px) and (max-width: 1263px) {
  .account_container {
    width: 90% !important;
    max-width: 90% !important;
  }
}
@media (max-width: 959px) {
  header {
    margin-left: 0 !important;
  }
  .propRow,
  .propRow .col-12 {
    padding-right: 0 !important;
    margin-right: 0 !important;
  }
}

@media (max-width: 500px) {
  .account_top_flex {
    margin-bottom: 77px !important;
  }

  .cp_wrapper {
    margin-top: 30px !important;
  }
  .Btns {
    font-size: 1.4rem !important;
  }
  .border {
    width: 95% !important;
    margin: 10px auto 0 !important;
    p {
      font-size: 1.6rem !important;
    }
  }
}
</style>