<template>
  <section id="account">
    <v-container class="account_container">
      <div class="account_top_flex">
        <AccountNav v-on:userLoggedOut="$emit('userLoggedOut')" />
        <v-row class="page_body">
          <div class="col-12">
            <header @click="reviews = !reviews">Reviews & Ratings</header>
          </div>
          <v-card class="border" v-if="!reviews">
            <div class="noReviews">
              <svg
                width="130"
                height="129"
                viewBox="0 0 130 129"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M27.024 38.494L29.4266 39.7182L29.4266 39.7182L27.024 38.494ZM29.3225 100.665L31.2292 102.571L31.2292 102.571L29.3225 100.665ZM97.3215 87.2196L96.0973 84.817L96.0973 84.817L97.3215 87.2196ZM104.392 80.1491L101.989 78.9249L101.989 78.925L104.392 80.1491ZM104.392 38.494L101.989 39.7182L101.989 39.7182L104.392 38.494ZM97.3215 31.4236L98.5457 29.021L97.3215 31.4236ZM34.0945 31.4236L32.8703 29.021L34.0945 31.4236ZM39.4245 90.5626L37.5178 88.6559L39.4245 90.5626ZM27.9571 55.5465C27.9571 50.9714 27.9592 47.7024 28.1686 45.1398C28.3754 42.6086 28.7709 41.0052 29.4266 39.7182L24.6214 37.2698C23.5137 39.4438 23.0275 41.836 22.7935 44.7006C22.562 47.5337 22.5641 51.0604 22.5641 55.5465H27.9571ZM27.9571 61.7669V55.5465H22.5641V61.7669H27.9571ZM22.4831 61.8479V88.6824H27.8761V61.8479H22.4831ZM22.4831 88.6824V98.9485H27.8761V88.6824H22.4831ZM22.4831 98.9485C22.4831 103.513 28.0017 105.799 31.2292 102.571L27.4158 98.7578C27.4314 98.7422 27.4885 98.7026 27.5699 98.6885C27.6367 98.6769 27.6831 98.6884 27.7097 98.6994C27.7362 98.7104 27.7771 98.7351 27.8161 98.7905C27.8638 98.8581 27.8761 98.9264 27.8761 98.9485H22.4831ZM31.2292 102.571L41.3312 92.4693L37.5178 88.6559L27.4158 98.7578L31.2292 102.571ZM80.2691 86.2865H43.2379V91.6795H80.2691V86.2865ZM96.0973 84.817C94.8104 85.4727 93.2069 85.8682 90.6758 86.075C88.1132 86.2844 84.8441 86.2865 80.2691 86.2865V91.6795C84.7551 91.6795 88.2818 91.6816 91.1149 91.4501C93.9796 91.2161 96.3718 90.7299 98.5457 89.6222L96.0973 84.817ZM101.989 78.925C100.697 81.4618 98.6342 83.5244 96.0973 84.817L98.5457 89.6222C102.097 87.8125 104.985 84.925 106.795 81.3733L101.989 78.925ZM103.459 63.0967C103.459 67.6717 103.457 70.9408 103.247 73.5034C103.041 76.0345 102.645 77.638 101.989 78.9249L106.795 81.3733C107.902 79.1994 108.388 76.8072 108.622 73.9426C108.854 71.1094 108.852 67.5827 108.852 63.0967H103.459ZM103.459 55.5465V63.0967H108.852V55.5465H103.459ZM101.989 39.7182C102.645 41.0052 103.041 42.6086 103.247 45.1398C103.457 47.7024 103.459 50.9715 103.459 55.5465H108.852C108.852 51.0604 108.854 47.5337 108.622 44.7006C108.388 41.836 107.902 39.4438 106.795 37.2698L101.989 39.7182ZM96.0973 33.8261C98.6342 35.1188 100.697 37.1813 101.989 39.7182L106.795 37.2698C104.985 33.7182 102.097 30.8306 98.5457 29.021L96.0973 33.8261ZM80.2691 32.3566C84.8441 32.3566 88.1132 32.3587 90.6758 32.5681C93.2069 32.7749 94.8104 33.1704 96.0973 33.8261L98.5457 29.021C96.3718 27.9133 93.9796 27.4271 91.1149 27.193C88.2818 26.9616 84.7551 26.9637 80.2691 26.9637V32.3566ZM51.1469 32.3566H80.2691V26.9637H51.1469V32.3566ZM35.3186 33.8261C36.6056 33.1704 38.2091 32.7749 40.7402 32.5681C43.3028 32.3587 46.5719 32.3566 51.1469 32.3566V26.9637C46.6609 26.9637 43.1342 26.9616 40.301 27.193C37.4364 27.4271 35.0442 27.9133 32.8703 29.021L35.3186 33.8261ZM29.4266 39.7182C30.7192 37.1813 32.7818 35.1188 35.3186 33.8261L32.8703 29.021C29.3186 30.8306 26.4311 33.7182 24.6214 37.2698L29.4266 39.7182ZM25.2201 59.1109C23.7085 59.1109 22.4831 60.3363 22.4831 61.8479H27.8761C27.8761 63.3148 26.687 64.5039 25.2201 64.5039V59.1109ZM41.3312 92.4693C41.8369 91.9636 42.5227 91.6795 43.2379 91.6795V86.2865C41.0924 86.2865 39.0348 87.1388 37.5178 88.6559L41.3312 92.4693ZM22.5641 61.7669C22.5641 60.3 23.7532 59.1109 25.2201 59.1109V64.5039C26.7317 64.5039 27.9571 63.2785 27.9571 61.7669H22.5641Z"
                  fill="#808494"
                />
                <path
                  d="M46.6797 51.0645L84.3047 51.0645"
                  stroke="#808494"
                  stroke-width="5.39299"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M46.6797 67.1914L73.5547 67.1914"
                  stroke="#808494"
                  stroke-width="5.39299"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <p class="noProp_review">
                You haven???t reviewed any properties yet
              </p>
              <p class="subtext">
                All the properties you have reviewed & rated will be shown here
              </p>
              <div class="cp_wrapper">
                <v-btn class="Btns" type="submit">Browse Properties</v-btn>
              </div>
            </div>
          </v-card>
          <PropertyReviewList v-else :edit="true" />
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

@media (max-width: 959px) {
  header {
    margin-left: 0 !important;
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