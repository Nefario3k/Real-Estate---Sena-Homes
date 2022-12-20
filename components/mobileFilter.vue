<template>
  <v-dialog
    v-model="showModal"
    :fullscreen="fullScreenModal"
    origin="center center"
    width="460"
    class="authDialog relative"
  >
    <v-card class="authCard" :class="{ fullscreen: fullScreenModal }">
      <div class="headerNnav">
        <div @click="showModal = false" class="controls">
          <svg
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M5 12L4.64645 11.6464L4.29289 12L4.64645 12.3536L5 12ZM17 12.5C17.2761 12.5 17.5 12.2761 17.5 12C17.5 11.7239 17.2761 11.5 17 11.5V12.5ZM8.64645 7.64645L4.64645 11.6464L5.35355 12.3536L9.35355 8.35355L8.64645 7.64645ZM4.64645 12.3536L8.64645 16.3536L9.35355 15.6464L5.35355 11.6464L4.64645 12.3536ZM5 12.5H17V11.5H5V12.5Z"
              fill="#BF9001"
            />
          </svg>
          <span>Back</span>
        </div>
        <div class="header"><span>Filters</span></div>
        <div class="controls">
          <span>Clear</span>
        </div>
      </div>
      <div class="modal_content">
        <form class="content_area">
          <v-row class="row_form">
            <!-- states  -->
            <div class="col-6">
              <!-- state  -->
              <v-menu
                :nudge-bottom="nudge_bottom"
                bottom
                offset-y
                :close-on-content-click="close_on_content_click"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown">
                    <span class="dropActive">State</span>
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
            <!-- city -->
            <div class="col-6">
              <!-- city -->
              <v-menu
                :nudge-bottom="nudge_bottom"
                bottom
                offset-y
                :close-on-content-click="close_on_content_click"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown">
                    <span class="dropActive">City</span>
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
            <!-- buy  -->
            <div class="col-12">
              <!-- buy  -->
              <v-menu
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
            <!-- property type  -->
            <div class="col-12">
              <!-- property type  -->
              <v-menu
                :nudge-bottom="nudge_bottom"
                bottom
                offset-y
                v-model="propbox"
                :close-on-content-click="close_on_content_click"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown mobile">
                    <span class="dropActive">Property</span>
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
                <v-list class="searchList proptype">
                  <!-- Residential -->
                  <v-list-item>
                    <div
                      @click="showTab(0)"
                      class="dropdown tabItem"
                      style="width: 100%"
                    >
                      <span class="dropActive">Residential</span>
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
                  </v-list-item>
                  <!-- Commercial -->
                  <v-list-item v-if="tab == null || tab == 1 || tab == 2">
                    <div
                      @click="showTab(1)"
                      class="dropdown tabItem"
                      style="width: 100%"
                    >
                      <span class="dropActive">Commercial</span>
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
                  </v-list-item>
                  <!-- Off-Plan -->
                  <v-list-item v-if="tab == null || tab == 2">
                    <div
                      @click="showTab(2)"
                      class="dropdown tabItem"
                      style="width: 100%"
                    >
                      <span class="dropActive">Off-Plan</span>
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
                  </v-list-item>
                  <v-tabs-items v-if="tab != null" v-model="tab">
                    <!-- Residential  -->
                    <v-tab-item>
                      <div class="gridMenu my-0">
                        <v-list-item class="gridItem">Apartment</v-list-item>
                        <v-list-item class="gridItem">Villa</v-list-item>
                        <v-list-item class="gridItem">Townhouse</v-list-item>
                        <v-list-item class="gridItem">Penthouse</v-list-item>
                        <v-list-item class="gridItem"
                          >Hotel Apartment</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Villa Compound</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Residential Plot</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Residential Floor</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Residential Building</v-list-item
                        >
                      </div>
                    </v-tab-item>
                    <!-- commercial  -->
                    <v-tab-item>
                      <div class="gridMenu my-0">
                        <v-list-item class="gridItem">Office</v-list-item>
                        <v-list-item class="gridItem">Shop</v-list-item>
                        <v-list-item class="gridItem">Warehouse</v-list-item>
                        <v-list-item class="gridItem"
                          >Commercial Building</v-list-item
                        >
                        <v-list-item class="gridItem">Factory</v-list-item>
                        <v-list-item class="gridItem">Showroom</v-list-item>
                        <v-list-item class="gridItem"
                          >Commercial Plot</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Commercial Floor</v-list-item
                        >
                      </div>
                    </v-tab-item>
                    <!-- off-plan  -->
                    <v-tab-item>
                      <div class="gridMenu my-0">
                        <v-list-item class="gridItem">Apartment</v-list-item>
                        <v-list-item class="gridItem">Villa</v-list-item>
                        <v-list-item class="gridItem">Townhouse</v-list-item>
                        <v-list-item class="gridItem">Penthouse</v-list-item>
                        <v-list-item class="gridItem"
                          >Hotel Apartment</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Villa Compound</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Residential Plot</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Residential Floor</v-list-item
                        >
                        <v-list-item class="gridItem"
                          >Residential Building</v-list-item
                        >
                      </div>
                    </v-tab-item>
                  </v-tabs-items>
                  <div
                    v-if="tab == null"
                    class="gridMenu mt-0 action"
                    style="gap: 8px"
                  >
                    <v-list-item class="px-0">
                      <v-btn class="Btn reset"><p>Reset</p></v-btn>
                    </v-list-item>
                    <v-list-item class="px-0">
                      <v-btn @click="propbox = false" class="Btn"
                        ><p>Done</p></v-btn
                      >
                    </v-list-item>
                  </div>
                  <!-- <v-list-item>

            <v-row>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
              <div class="col-6">whuhvd</div>
            </v-row>
          </v-list-item> -->
                </v-list>
              </v-menu>
            </div>
            <!-- Beds and bath  -->
            <div class="col-12">
              <v-menu
                :nudge-left="bednbath"
                :nudge-bottom="nudge_bottom"
                bottom
                v-model="bedbox"
                offset-y
                :close-on-content-click="close_on_content_click"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown mobile">
                    <span class="dropActive">Beds & Baths</span>
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
                <v-list class="searchList bed">
                  <v-list-item class="bedTitle">
                    <p>Beds</p>
                  </v-list-item>
                  <div class="gridMenu mt-0">
                    <v-list-item class="gridItem lg">Studio</v-list-item>
                    <v-list-item class="gridItem">1</v-list-item>
                    <v-list-item class="gridItem">2</v-list-item>
                    <v-list-item class="gridItem">3</v-list-item>
                    <v-list-item class="gridItem">4</v-list-item>
                    <v-list-item class="gridItem">5</v-list-item>
                    <v-list-item class="gridItem">6</v-list-item>
                    <v-list-item class="gridItem">7</v-list-item>
                    <v-list-item class="gridItem">8+</v-list-item>
                  </div>
                  <v-list-item class="bedTitle">
                    <p>Baths</p>
                  </v-list-item>
                  <div class="gridMenu mt-0 baths">
                    <v-list-item class="gridItem">1</v-list-item>
                    <v-list-item class="gridItem">2</v-list-item>
                    <v-list-item class="gridItem">3</v-list-item>
                    <v-list-item class="gridItem">4</v-list-item>
                    <v-list-item class="gridItem">5</v-list-item>
                    <v-list-item class="gridItem">6+</v-list-item>
                  </div>
                  <div class="gridMenu mt-0 action">
                    <v-list-item>
                      <v-btn class="Btn reset"><p>Reset</p></v-btn>
                    </v-list-item>
                    <v-list-item>
                      <v-btn @click="bedbox = false" class="Btn"
                        ><p>Done</p></v-btn
                      >
                    </v-list-item>
                  </div>
                </v-list>
              </v-menu>
            </div>
            <!-- prices  -->
            <div class="col-12">
              <v-menu
                :nudge-left="nudge_left"
                :nudge-bottom="nudge_bottom"
                bottom
                v-model="pricebox"
                offset-y
                :close-on-content-click="close_on_content_click"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown mobile">
                    <span class="dropActive">Prices</span>
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
                <v-list class="searchList prices">
                  <div class="gridMenu">
                    <v-list-item>
                      <p>Minimum</p>
                      <v-menu bottom offset-y :max-height="204">
                        <template v-slot:activator="{ on, attrs }">
                          <div v-bind="attrs" v-on="on" class="">
                            <input type="text" value="0" />
                          </div>
                        </template>
                        <v-list class="searchList featured">
                          <v-list-item>
                            <v-list-item-title>20,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>30,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>40,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>50,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>60,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>70,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>80,000</v-list-item-title>
                          </v-list-item>
                        </v-list>
                      </v-menu>
                    </v-list-item>
                    <v-list-item>
                      <p>Maximum</p>
                      <v-menu bottom offset-y :max-height="204">
                        <template v-slot:activator="{ on, attrs }">
                          <div v-bind="attrs" v-on="on" class="">
                            <input type="text" value="Any" />
                          </div>
                        </template>
                        <v-list class="searchList featured">
                          <v-list-item>
                            <v-list-item-title>Any</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>400,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>500,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>600,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>700,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>800,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>900,000</v-list-item-title>
                          </v-list-item>
                          <v-list-item>
                            <v-list-item-title>1M</v-list-item-title>
                          </v-list-item>
                        </v-list>
                      </v-menu>
                    </v-list-item>
                    <v-list-item>
                      <v-btn class="Btn reset"><p>Reset</p></v-btn>
                    </v-list-item>
                    <v-list-item>
                      <v-btn @click="pricebox = false" class="Btn"
                        ><p>Done</p></v-btn
                      >
                    </v-list-item>
                  </div>
                </v-list>
              </v-menu>
            </div>
            <!-- input field  -->
            <div class="col-12">
              <input
                placeholder="Add relevant keywords..."
                type=""
                name=""
                value=""
              />
            </div>
            <!-- amenties  -->
            <div class="col-12">
              <v-menu :nudge-bottom="nudge_bottom" bottom offset-y>
                <template v-slot:activator="{ on, attrs }">
                  <div
                    v-bind="attrs"
                    v-on="on"
                    class="dropdown"
                    style="width: 100%"
                  >
                    <span class="dropActive">Amenties</span>
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
                <v-list class="searchList" flat :elevation="0">
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
            <div class="col-12">
              <v-menu
                :nudge-bottom="nudge_bottom"
                bottom
                offset-y
                :max-height="204"
              >
                <template v-slot:activator="{ on, attrs }">
                  <div v-bind="attrs" v-on="on" class="dropdown mobile">
                    <span class="dropActive">Featured</span>
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
                    <v-list-item-title>Newest First</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Oldest First</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Lowest price first</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Highest price first</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Newest First</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Oldest First</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Lowest price first</v-list-item-title>
                  </v-list-item>
                  <v-list-item>
                    <v-list-item-title>Highest price first</v-list-item-title>
                  </v-list-item>
                </v-list>
              </v-menu>
            </div>
          </v-row>
          <footer class="footer">
            <v-btn class="Btn"><p>Search</p></v-btn>
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
      propbox: false,
      bedbox: false,
      pricebox: false,
      tab: null,
      fullScreenModal: true,
      close_on_content_click: false,
      min_width: 325,
      nudge_bottom: 10,
      nudge_left: "0%",
      bednbath: "0%",
    };
  },
  methods: {
    showFilterModal() {
      this.showModal = true;
    },
    showTab(type) {
      if (this.tab == type) {
        this.tab = null;
      } else {
        this.tab = type;
      }
    },
  },
};
</script>

<style lang="scss" scoped>
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
@keyframes transIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}
@keyframes transOut {
  from {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}
.headerNnav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 34px 12px 0;
  div.controls {
    display: flex;
    align-items: center;
    cursor: pointer;
    span {
      font-weight: 500;
      font-size: 1.4rem;
      color: var(--primary-color);
    }
  }
  div.header {
    span {
      font-weight: 500;
      font-size: 1.8rem;
      color: var(--secondary-color);
    }
  }
}
.col-12,
.col-6 {
  padding-bottom: 0;
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
  &.tabItem {
    animation: transIn 0.2s linear 0s;
  }
}

.dropdown span {
  color: var(--faded-color);
  font-weight: 500;
  font-size: 1.8rem;
}

.dropdown span.dropActive {
  color: var(--faded-color);
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
input {
  padding: 0 10px !important;
  width: 100%;
  background-color: transparent;
  height: 4.9rem !important;
  font-size: 1.8rem !important;
  color: var(--secondary-color);
  -moz-appearance: none;
  /* Firefox */
  -webkit-appearance: none;
  /* Safari and Chrome */
  appearance: none;
  outline: none !important;
  border: 1px solid var(--primaryLte-color) !important;
  border-radius: 0;
}
input:focus {
  -moz-appearance: none;
  /* Firefox */
  -webkit-appearance: none;
  /* Safari and Chrome */
  appearance: none;
  outline: none !important;
  border: 1px solid var(--primary-color) !important;
}
input::placeholder {
  color: rgba(190, 190, 190, 0.5);
  font-weight: 500;
  font-size: 1.8rem;
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
  &.proptype {
    .gridMenu {
      .gridItem {
        animation: transIn 0.2s linear 0s;
      }
    }
  }
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
.searchList.prices {
  .gridMenu {
    padding: 18;
    margin: 0;
    column-gap: 9px;
    row-gap: 23px;
    .v-list-item {
      flex-direction: column;
      align-items: flex-start;
      padding: 0;
      min-height: auto;
    }
    input {
      text-align: center;
    }
  }
}
.searchList.bed {
  .gridMenu {
    grid-template-columns: repeat(6, 4.8rem);
    padding-right: 58px;
    .gridItem {
      height: 3.2rem;
      border: 1px solid var(--primaryLte-color);
      font-weight: 400;
      color: #000;
    }
    .gridItem.lg {
      grid-column: span 2;
    }
  }
  .gridMenu.baths {
    grid-template-columns: repeat(5, 4.8rem);
  }
  .gridMenu.action {
    grid-template-columns: repeat(2, 1fr);
    padding-right: 16px;
    .v-list-item {
      padding: 0;
    }
  }
}
.footer {
  position: absolute;
  bottom: 0;
  left: 12px;
  width: 95% !important;
}
@media (max-width: 533px) {
  .searchList.bed {
    .gridMenu {
      grid-template-columns: repeat(5, 4.8rem);
    }
  }
}
@media (max-width: 363px) {
  .searchList.bed {
    .gridMenu,
    .gridMenu.baths {
      grid-template-columns: repeat(4, 4.8rem);
    }
  }
}
@media (max-width: 297px) {
  .searchList.bed {
    .gridMenu,
    .gridMenu.baths {
      grid-template-columns: repeat(3, 4.8rem);
    }
  }
}
</style>