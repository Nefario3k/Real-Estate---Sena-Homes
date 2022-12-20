<template>
  <div id="faq">
    <v-container>
      <v-row no-gutters>
        <v-col class="col-12 col-md-6 col-lg-6 col-xl-6">
          <h5 data-aos="fade-right" data-aos-duration="500">FAQ</h5>
          <h3 data-aos="fade-up" data-aos-duration="500">
            Frequently Asked Questions
          </h3>
          <p data-aos="fade-up" data-aos-duration="500">
            Have a question? We are here to help you
          </p>
          <nuxt-link
            to="/contact-us"
            class="mobileHidden"
            style="text-decoration: none"
          >
            <v-btn data-aos="fade-up" data-aos-duration="500" class="custom-btn"
              >Contact Us</v-btn
            >
          </nuxt-link>
        </v-col>
        <v-col class="col-12 col-md-6 col-lg-6 col-xl-6">
          <template>
            <v-row justify="center" style="padding-right: 0">
              <v-expansion-panels
                accordion
                data-aos="fade-up"
                data-aos-duration="500"
              >
                <v-expansion-panel
                  v-for="(item, i) in faq"
                  :key="i"
                  @click="toggleUpDown(i)"
                >
                  <v-expansion-panel-header>
                    {{ item.question }}
                    <template v-slot:actions>
                      <div class="iconsvg">
                        <svg
                          :class="{ activeIcon: isActiveIndex == i }"
                          width="12"
                          height="8"
                          viewBox="0 0 12 8"
                          fill="none"
                          xmlns="http://www.w3.org/2000/svg"
                        >
                          <path
                            fill-rule="evenodd"
                            clip-rule="evenodd"
                            d="M5.04535 7.14L0.249351 1.658C-0.316649 1.013 0.143351 3.69899e-07 1.00235 3.69899e-07H10.5944C10.987 -0.000336283 11.3435 0.229148 11.5058 0.586693C11.6681 0.944239 11.6061 1.36367 11.3474 1.659L6.55135 7.139C6.36145 7.35631 6.08694 7.48098 5.79835 7.48098C5.50976 7.48098 5.23525 7.35631 5.04535 7.139V7.14Z"
                            fill="#F8F5F0"
                          />
                        </svg>
                      </div>
                      <!-- <img
                        :class="{ activeIcon: isActiveIndex == i }"
                        src="./images/svg/circle-down.svg"
                        alt=""
                      /> -->
                    </template>
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    {{ item.answer }}
                  </v-expansion-panel-content>
                </v-expansion-panel>
              </v-expansion-panels>
            </v-row>
          </template>
        </v-col>
        <v-col
          class="col-12 text-center hidden mobilectu"
          style="margin-top: 40px"
        >
          <p
            data-aos="fade-up"
            data-aos-duration="500"
            style="margin-bottom: 21px"
          >
            Still have questions?
          </p>
          <nuxt-link to="/contact-us" style="text-decoration: none">
            <v-btn data-aos="fade-up" data-aos-duration="500" class="custom-btn"
              >Contact Us</v-btn
            >
          </nuxt-link>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    align: "start",
    faq: [
      {
        question: "What is the first step in the home buying process?",
        answer:
          "No. We don't ask you for your credit card up front, so you'll only be charged when you decide to continue after your trial ends. If not, your trial will expire automatically, and your account data will be deleted.",
      },
      {
        question: "How long does it take to buy a home?",
        answer:
          "No. We don't ask you for your credit card up front, so you'll only be charged when you decide to continue after your trial ends. If not, your trial will expire automatically, and your account data will be deleted.",
      },
      {
        question: "How long can the seller take to respond to my offer?",
        answer:
          "No. We don't ask you for your credit card up front, so you'll only be charged when you decide to continue after your trial ends. If not, your trial will expire automatically, and your account data will be deleted.",
      },
      {
        question: "How much do i have to pay an agent to help me buy a house?",
        answer:
          "No. We don't ask you for your credit card up front, so you'll only be charged when you decide to continue after your trial ends. If not, your trial will expire automatically, and your account data will be deleted.",
      },
    ],
    isActiveIndex: null,
  }),
  methods: {
    toggleUpDown(i) {
      if (this.isActiveIndex == i) this.isActiveIndex = null;
      else this.isActiveIndex = i;
    },
  },
};
</script>
<style lang="scss" scoped>
#faq {
  min-height: 738px;
  background: #1c212b;
  background-image: url(./images/svg/faq-vector-1.svg),
    url(./images/svg/faq-vector-2.svg);
  background-position: top left, bottom right;
  background-repeat: no-repeat;
  padding-top: 10.5rem;

  .row {
    margin: 0;
    padding: 0 1rem;

    .col {
      h5 {
        font-weight: 400;
        font-size: 16px;
        line-height: 32px;
        letter-spacing: 3px;
        color: var(--primary-color);
        margin-bottom: 1.7rem;
      }

      h3 {
        font-weight: 700;
        font-size: 40px;
        line-height: 48px;
        color: #ffffff;
        margin-bottom: 3rem;
      }

      p {
        font-weight: 400;
        font-size: 16px;
        line-height: 32px;
        color: rgba(255, 255, 255, 0.64);
        margin-bottom: 4rem;
      }
      .custom-btn {
        width: 213px;
        height: 50px;
        font-weight: 700;
        font-size: 16px;
        line-height: 36px;
        color: #f8f5f0;
        background: var(--primary-color);
        text-transform: capitalize;
        border-radius: 0;
      }

      .v-expansion-panels {
        border-radius: 0;
      }

      .v-expansion-panel-header {
        font-weight: 700;
        font-size: 16px;
        line-height: 32px;
        color: #ffffff;
        padding: 24px;
        align-items: start;

        &--active {
          color: var(--gei-color);
          background: #f8f5f0;
          // box-shadow: 0px 32px 64px rgba(57, 20, 0, 0.04);
        }
        &__icon {
          .iconsvg {
            width: 3.2rem;
            height: 3.2rem;
            background: var(--primary-color);
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            svg {
              transition: all 0.3s ease-in-out;
            }
          }
        }

        .activeIcon {
          rotate: -180deg;
          transition: all 0.3s ease-in-out;
        }
      }

      .v-expansion-panel-content {
        font-weight: 400;
        font-size: 16px;
        line-height: 32px;
        color: rgba(57, 20, 0, 0.64);
        background: var(--secondary-color);
      }

      .theme--light.v-expansion-panels .v-expansion-panel {
        background-color: transparent;
        border: 1px solid #3a3c56;
      }

      .v-expansion-panel-header--active ~ .v-expansion-panel-content {
        background: #f8f5f0;
        box-shadow: 0px 32px 64px rgba(57, 20, 0, 0.04);
      }
    }
  }

  .v-expansion-panel-content {
    font-weight: 400;
    font-size: 16px;
    line-height: 32px;
    color: rgba(57, 20, 0, 0.64);
    background: var(--secondary-color);
  }

  .v-expansion-panel-header--active ~ .v-expansion-panel-content {
    background: #f8f5f0;
    box-shadow: 0px 32px 64px rgba(57, 20, 0, 0.04);
  }
}

@media (max-width: 959px) {
  #faq {
    height: 100%;
    padding: 3.5rem 0 7.5rem;
    background-image: url(./images/svg/faq-vector-1-mobile.svg),
      url(./images/svg/faq-vector-2-mobile.svg);

    .row {
      .col {
        text-align: center;

        h3 {
          font-weight: 800;
          font-size: 32px;
        }

        .v-expansion-panel-header {
          &__icon {
            // margin-top: 4px;
          }
        }

        .v-expansion-panel-content {
          font-weight: 400;
          font-size: 14px;
          line-height: 32px;
          text-align: left;
        }

        .theme--light.v-expansion-panels .v-expansion-panel {
          border: 0.5px solid #f8f5f0;
        }
      }
    }
  }
}
@media (max-width: 959px) {
  .mobileHidden {
    display: none !important;
  }
  .mobilectu {
    display: block !important;
  }
}
</style>
