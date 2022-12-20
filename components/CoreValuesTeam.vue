<template>
  <v-container fluid style="">
    <section class="valueSection relative">
      <div class="core-values">
        <p
          data-aos="fade-up"
          data-aos-duration="400"
          class="text-center core-value-intro"
        >
          What we believe
        </p>
        <h4
          data-aos="fade-left"
          data-aos-duration="800"
          class="text-center mb-8"
        >
          Our Core Values
        </h4>
        <aside class="coreValuesContainer relative">
          <v-tabs
            data-aos="fade-left"
            data-aos-duration="800"
            center-active
            background-color="transparent"
            centered
            height="230"
            hide-slider
            :show-arrows="true"
            v-model="tabz"
            class="core_wrapper"
          >
            <v-tab
              :class="{ active: tabz == 0 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Accountability</p>
            </v-tab>
            <v-tab
              :class="{ active: tabz == 1 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Transparency</p>
            </v-tab>
            <v-tab
              :class="{ active: tabz == 2 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Passion</p>
            </v-tab>
            <v-tab
              :class="{ active: tabz == 3 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Professionalism</p>
            </v-tab>
            <v-tab
              :class="{ active: tabz == 4 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Accountability</p>
            </v-tab>
            <v-tab
              :class="{ active: tabz == 5 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Transparency</p>
            </v-tab>
            <v-tab
              :class="{ active: tabz == 6 }"
              class="
                core_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/icon_values.png" alt="core-value-icon" />
              <p class="font-weight-bold">Passion</p>
            </v-tab>
          </v-tabs>
          <div @click="switchTabz('next')" class="next slideBtn">
            <svg
              width="50"
              height="50"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect x="0.5" y="0.5" width="49" height="49" stroke="#A98453" />
              <path
                d="M25.0002 35L35.0002 25L25.0002 15"
                stroke="#A98453"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M15.0002 25L35.0002 25"
                stroke="#A98453"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <div
            @click="switchTabz('prev')"
            class="prev slideBtn"
            :class="{ active: tabz > 0 }"
          >
            <svg
              width="50"
              height="50"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect x="0.5" y="0.5" width="49" height="49" stroke="#7B7B7B" />
              <path
                d="M24.9999 15L14.9999 25L24.9999 35"
                stroke="#7B7B7B"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M34.9999 25H14.9999"
                stroke="#7B7B7B"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </aside>
      </div>
    </section>
    <section class="team">
      <div class="teamContentwrapper">
        <h3 data-aos="fade-up" data-aos-duration="400" class="text-center">
          The Team
        </h3>
        <p
          data-aos="fade-right"
          data-aos-duration="800"
          style="color: var(--secondary-color); line-height: 37px !important"
          class="team-intro text-center mt-4 mb-12"
        >
          The SENA HOMES REAL ESTATE management team consists of highly
          respected individuals with years of professional experience and a
          solid industry reputation.
        </p>
        <aside class="team_container relative">
          <v-tabs
            data-aos="fade-right"
            data-aos-duration="800"
            center-active
            background-color="white"
            centered
            height="400"
            hide-slider
            :show-arrows="true"
            v-model="tabs"
            class="team_wrapper"
          >
            <v-tab
              :class="{ active: tabs == 0 }"
              class="
                team_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/team1.png" alt="team photo" />
              <p class="staff-name">Grant Marshall</p>
              <span class="role">Agents</span>
            </v-tab>
            <v-tab
              :class="{ active: tabs == 1 }"
              class="
                team_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/team2.png" alt="team photo" />
              <p class="staff-name">Grant Marshall</p>
              <span class="role">Agents</span>
            </v-tab>
            <v-tab
              :class="{ active: tabs == 2 }"
              class="
                team_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/team3.png" alt="team photo" />
              <p class="staff-name">Grant Marshall</p>
              <span class="role">Agents</span>
            </v-tab>
            <v-tab
              :class="{ active: tabs == 3 }"
              class="
                team_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/team1.png" alt="team photo" />
              <p class="staff-name">Grant Marshall</p>
              <span class="role">Agents</span>
            </v-tab>
            <v-tab
              :class="{ active: tabs == 4 }"
              class="
                team_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/team2.png" alt="team photo" />
              <p class="staff-name">Grant Marshall</p>
              <span class="role">Agents</span>
            </v-tab>
            <v-tab
              :class="{ active: tabs == 5 }"
              class="
                team_items
                d-flex
                flex-column
                justify-center
                align-center
                py-12
              "
            >
              <img src="images/pngs/team3.png" alt="team photo" />
              <p class="staff-name">Grant Marshall</p>
              <span class="role">Agents</span>
            </v-tab>
          </v-tabs>
          <div @click="switchTabs('next')" class="next slideBtn">
            <svg
              width="50"
              height="50"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect x="0.5" y="0.5" width="49" height="49" stroke="#A98453" />
              <path
                d="M25.0002 35L35.0002 25L25.0002 15"
                stroke="#A98453"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M15.0002 25L35.0002 25"
                stroke="#A98453"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <div
            @click="switchTabs('prev')"
            class="prev slideBtn"
            :class="{ active: tabs > 0 }"
          >
            <svg
              width="50"
              height="50"
              viewBox="0 0 50 50"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect x="0.5" y="0.5" width="49" height="49" stroke="#7B7B7B" />
              <path
                d="M24.9999 15L14.9999 25L24.9999 35"
                stroke="#7B7B7B"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M34.9999 25H14.9999"
                stroke="#7B7B7B"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </aside>
      </div>
    </section>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      tabs: 1,
      tabz: null,
      tab_height: 335,
    };
  },
  methods: {
    switchTabs(type) {
      switch (type) {
        case "prev":
          if (this.tabs === "" || this.tabs === null || this.tabs == 0) {
            return;
          } else {
            this.tabs = this.tabs - 1;
          }
          break;
        case "next":
          this.tabs = this.tabs + 1;
          break;

        default:
          break;
      }
    },
    switchTabz(type) {
      switch (type) {
        case "prev":
          if (this.tabz === "" || this.tabz === null || this.tabz == 0) {
            return;
          } else {
            this.tabz = this.tabz - 1;
          }
          break;
        case "next":
          this.tabz = this.tabz + 1;
          break;

        default:
          break;
      }
    },
  },
};
</script>
<style lang="scss" scoped>
div.container {
  padding: 0px;
}

.valueSection {
  background-color: #f7f4f2;
  background-image: url(./images/svg/arrowHead.svg"),
    url(./images/pngs/dotted_bg2.png"), url(./images/pngs/dotted_bg2.png");
  background-position: bottom center, top left, bottom right;
  overflow: hidden;

  .dotted_bg1 {
    position: absolute;
    top: -2rem;
    left: -2rem;
  }
}

.core-values {
  width: 85%;
  margin: auto;
  padding-top: 69px;
  padding-bottom: 114px;
  overflow: hidden;
}

.core-value-intro {
  color: #bf9001;
  text-transform: uppercase;
  font-size: 1.8rem;
}

h4 {
  font-size: 4rem;
}
.team {
  background-image: url(./images/pngs/dotted_bg.png");
  background-position: bottom right;
  overflow: hidden;
  .teamContentwrapper {
    padding: 124px 0;
    width: 85%;
    margin: auto;
  }
}

.coreValuesContainer {
  z-index: 2;
  .core_wrapper {
    width: 85%;
    margin: auto;
    .core_items {
      background-color: #f7f4f2;
      min-width: 21.5rem;
      text-align: center;
      z-index: 3;
      border: 1px solid var(--primary-color);
      margin-right: 55px;
      gap: 14px;
      p {
        font-weight: 500;
        font-size: 2rem;
        color: var(--secondary-color);
        margin-bottom: 0;
        text-transform: none;
      }
      &.active {
        p {
          color: var(--primary-color);
        }
      }
    }
  }
  .slideBtn {
    position: absolute;

    &.next {
      right: 0;
      top: 40%;
      cursor: pointer;

      svg rect {
        stroke: var(--carousel-btn);
      }

      svg path {
        stroke: var(--carousel-btn);
      }
    }

    &.prev {
      left: 0;
      top: 40%;
      cursor: pointer;

      &.active {
        svg rect {
          stroke: var(--carousel-btn);
          transition: all 0.2s linear;
        }

        svg path {
          stroke: var(--carousel-btn);
          transition: all 0.2s linear;
        }
      }
    }
  }
}

.team_container {
  z-index: 2;
  margin-bottom: 112px;

  .team_wrapper {
    width: 85%;
    margin: 0 auto;

    .team_items {
      background-color: #f7f4f2;
      min-width: 35rem;
      text-align: center;
      z-index: 3;
      margin-right: 30px;

      &.active {
        border: 1px solid var(--primary-color);
        color: var(--primary-color) !important;
      }

      & .staff-name {
        margin: 0px;
        margin-top: 2rem;
        font-size: 2.4rem;
        font-weight: 500;
      }

      & .role {
        color: #7b7b7b;
        font-size: 1.8rem;
      }

      img {
        border-radius: 50%;
        max-width: 12.5rem;
      }
    }
  }

  .slideBtn {
    position: absolute;

    &.next {
      right: 0;
      top: 47%;
      cursor: pointer;

      svg rect {
        stroke: var(--carousel-btn);
      }

      svg path {
        stroke: var(--carousel-btn);
      }
    }

    &.prev {
      left: 0;
      top: 47%;
      cursor: pointer;

      &.active {
        svg rect {
          stroke: var(--carousel-btn);
          transition: all 0.2s linear;
        }

        svg path {
          stroke: var(--carousel-btn);
          transition: all 0.2s linear;
        }
      }
    }
  }
}

// => 'sm': '640px',
@media (min-width: 640px) {
}

// => 'md': '768px',
@media (min-width: 768px) {
  div.container {
    padding: 0px;
  }

  .core-values {
    position: relative;

    .dotted_bg1 {
      position: absolute;
      top: -2rem;
      left: -2rem;
    }
  }

  .core-value-intro {
    color: #bf9001;
    text-transform: uppercase;
    font-size: 1.8rem;
  }

  h4 {
    font-size: 4rem;
  }

  .core-values-list {
    text-align: center;
    width: 80%;
    margin: auto;

    div {
      border: 1px solid #bf9001;
      max-width: 21.5rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      img {
        max-width: 12.6rem;
      }

      p {
        margin-top: 2rem;
      }
    }
  }

  .team {
    background-color: #fff;
    position: relative;

    h3 {
      font-size: 4rem;
    }

    .team-intro {
      width: 60%;
      margin: auto;
      font-size: 1.8rem;
    }

    .team-list {
      width: 80%;
      margin: auto;

      div.col {
        background-color: #f7f4f2;
        max-width: 35rem;
        // border: 1px solid rgb(142, 141, 235);
        text-align: center;
        z-index: 3;

        &.active {
          border: 1px solid #bf9001;
        }

        & .staff-name {
          margin: 0px;
          margin-top: 2rem;
          font-size: 2.4rem;
          font-weight: 500;
        }

        & .role {
          color: #7b7b7b;
          font-size: 1.8rem;
        }

        img {
          border-radius: 50%;
          max-width: 12.5rem;
        }
      }
    }
  }
}

// => 'lg': '1024px',
@media (min-width: 1024px) {
}

// => 'xl': '1280px',
@media (min-width: 1280px) {
}

// => '2xl': '1536px',
@media (min-width: 1536px) {
}

@media (max-width: 500px) {
  .team {
    background-position: bottom -1rem right -2rem !important;
    background-size: 50% !important;
    .teamContentwrapper {
      width: 90% !important;
      padding: 54px 0 72px !important;
      h3 {
        font-size: 2.4rem !important;
      }
      p.team-intro {
        font-size: 1.6rem !important;
      }
      .team_wrapper {
        width: 90% !important;

        .team_items {
          min-width: 30rem !important;
          padding: 0 20px !important;
        }
      }
      .slideBtn {
        &.next {
          bottom: -6.9rem !important;
          right: 31% !important;
          top: auto !important;

          svg rect {
            fill: var(--carousel-btn);
          }
          svg path {
            stroke: #fff !important;
          }
        }

        &.prev {
          bottom: -6.9rem !important;
          left: 31% !important;
          top: auto !important;
          &.active {
            svg rect {
              fill: var(--carousel-btn);
            }
            svg path {
              stroke: #fff !important;
            }
          }
        }
      }
    }
  }
  .valueSection {
    background-size: 75%, 20%, 20%;
    .core-values {
      //  padding-top: 69px !important;
      padding-bottom: 154px !important;
      .core-value-intro {
        font-size: 1.6rem !important;
      }
      h4 {
        font-size: 2.4rem;
      }
      .coreValuesContainer {
        .slideBtn {
          &.next {
            bottom: -6.9rem !important;
            right: 30% !important;
            top: auto !important;

            svg rect {
              fill: var(--carousel-btn);
            }
            svg path {
              stroke: #fff !important;
            }
          }

          &.prev {
            bottom: -6.9rem !important;
            left: 30% !important;
            top: auto !important;
            &.active {
              svg rect {
                fill: var(--carousel-btn);
              }
              svg path {
                stroke: #fff !important;
              }
            }
          }
        }
      }
    }
  }
}
</style>