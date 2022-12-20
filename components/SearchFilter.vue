<template>
  <v-container class="filterContainer">
    <div class="search_grid">
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
      <!-- state  -->
      <v-menu
        allow-overflow
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
      <!-- city -->
      <v-menu
        allow-overflow
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
      <!-- featured  -->
      <v-menu
        allow-overflow
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
      <!-- filters  -->
      <v-menu
        allow-overflow
        :nudge-left="nudge_left"
        :nudge-bottom="nudge_bottom"
        bottom
        offset-y
        :close-on-content-click="close_on_content_click"
        :min-width="min_width"
        :max-height="515"
      >
        <template v-slot:activator="{ on, attrs }">
          <div v-bind="attrs" v-on="on" class="dropdown mobile">
            <span class="dropActive">Filters</span>
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path d="M12 7L20 7" stroke="#222222" stroke-linecap="round" />
              <path d="M4 7L8 7" stroke="#222222" stroke-linecap="round" />
              <path d="M17 17L20 17" stroke="#222222" stroke-linecap="round" />
              <path d="M4 17L12 17" stroke="#222222" stroke-linecap="round" />
              <circle
                cx="10"
                cy="7"
                r="2"
                transform="rotate(90 10 7)"
                stroke="#222222"
                stroke-linecap="round"
              />
              <circle
                cx="15"
                cy="17"
                r="2"
                transform="rotate(90 15 17)"
                stroke="#222222"
                stroke-linecap="round"
              />
            </svg>
          </div>
        </template>
        <v-list class="searchList">
          <v-list-item class="">
            <input
              type=""
              name=""
              value=""
              placeholder="Add relevant keywords..."
            />
          </v-list-item>
          <v-list-item>
            <v-menu allow-overflow :nudge-bottom="nudge_bottom" bottom offset-y>
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
          </v-list-item>
          <div class="gridMenu">
            <v-list-item class="gridItem">Central A/C</v-list-item>
            <v-list-item class="gridItem">View of Landmark</v-list-item>
            <v-list-item class="gridItem">Maids Room</v-list-item>
            <v-list-item class="gridItem">Built in Wardrobes</v-list-item>
            <v-list-item class="gridItem">Study</v-list-item>
            <v-list-item class="gridItem">Balcony or Terrace</v-list-item>
            <v-list-item class="gridItem">Walk-in Closet</v-list-item>
            <v-list-item class="gridItem">Private Pool</v-list-item>
            <v-list-item class="gridItem">Covered Parking</v-list-item>
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
      <!-- filters Mobile  -->
      <div @click="showModal('filter')" class="dropdown noShow">
        <span class="dropActive">Filters</span>
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path d="M12 7L20 7" stroke="#222222" stroke-linecap="round" />
          <path d="M4 7L8 7" stroke="#222222" stroke-linecap="round" />
          <path d="M17 17L20 17" stroke="#222222" stroke-linecap="round" />
          <path d="M4 17L12 17" stroke="#222222" stroke-linecap="round" />
          <circle
            cx="10"
            cy="7"
            r="2"
            transform="rotate(90 10 7)"
            stroke="#222222"
            stroke-linecap="round"
          />
          <circle
            cx="15"
            cy="17"
            r="2"
            transform="rotate(90 15 17)"
            stroke="#222222"
            stroke-linecap="round"
          />
        </svg>
      </div>
      <MobileFilter ref="filterModal" />
      <!-- property type  -->
      <v-menu
        allow-overflow
        v-model="propsbox"
        :nudge-left="nudge_left"
        :nudge-bottom="nudge_bottom"
        bottom
        offset-y
        :close-on-content-click="close_on_content_click"
        :min-width="min_width"
        :max-height="515"
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
                <v-list-item class="gridItem">Hotel Apartment</v-list-item>
                <v-list-item class="gridItem">Villa Compound</v-list-item>
                <v-list-item class="gridItem">Residential Plot</v-list-item>
                <v-list-item class="gridItem">Residential Floor</v-list-item>
                <v-list-item class="gridItem">Residential Building</v-list-item>
              </div>
            </v-tab-item>
            <!-- commercial  -->
            <v-tab-item>
              <div class="gridMenu my-0">
                <v-list-item class="gridItem">Office</v-list-item>
                <v-list-item class="gridItem">Shop</v-list-item>
                <v-list-item class="gridItem">Warehouse</v-list-item>
                <v-list-item class="gridItem">Commercial Building</v-list-item>
                <v-list-item class="gridItem">Factory</v-list-item>
                <v-list-item class="gridItem">Showroom</v-list-item>
                <v-list-item class="gridItem">Commercial Plot</v-list-item>
                <v-list-item class="gridItem">Commercial Floor</v-list-item>
              </div>
            </v-tab-item>
            <!-- off-plan  -->
            <v-tab-item>
              <div class="gridMenu my-0">
                <v-list-item class="gridItem">Apartment</v-list-item>
                <v-list-item class="gridItem">Villa</v-list-item>
                <v-list-item class="gridItem">Townhouse</v-list-item>
                <v-list-item class="gridItem">Penthouse</v-list-item>
                <v-list-item class="gridItem">Hotel Apartment</v-list-item>
                <v-list-item class="gridItem">Villa Compound</v-list-item>
                <v-list-item class="gridItem">Residential Plot</v-list-item>
                <v-list-item class="gridItem">Residential Floor</v-list-item>
                <v-list-item class="gridItem">Residential Building</v-list-item>
              </div>
            </v-tab-item>
          </v-tabs-items>
          <div v-if="tab == null" class="gridMenu mt-0 action" style="gap: 8px">
            <v-list-item class="px-0">
              <v-btn class="Btn reset"><p>Reset</p></v-btn>
            </v-list-item>
            <v-list-item class="px-0">
              <v-btn @click="propsbox = false" class="Btn"><p>Done</p></v-btn>
            </v-list-item>
          </div>
        </v-list>
      </v-menu>
      <!-- Beds and bath  -->
      <v-menu
        v-model="bedsbox"
        allow-overflow
        :nudge-left="bednbath"
        :nudge-bottom="nudge_bottom"
        bottom
        offset-y
        :close-on-content-click="close_on_content_click"
        :min-width="min_width"
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
              <v-btn @click="bedsbox = false" class="Btn"><p>Done</p></v-btn>
            </v-list-item>
          </div>
        </v-list>
      </v-menu>
      <!-- prices  -->
      <v-menu
        v-model="pricesbox"
        allow-overflow
        :nudge-left="nudge_left"
        :nudge-bottom="nudge_bottom"
        bottom
        offset-y
        :close-on-content-click="close_on_content_click"
        :min-width="min_width"
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
              <v-menu allow-overflow bottom offset-y :max-height="204">
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
              <v-menu allow-overflow bottom offset-y :max-height="204">
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
              <v-btn @click="pricesbox = false" class="Btn"><p>Done</p></v-btn>
            </v-list-item>
          </div>
        </v-list>
      </v-menu>
      <v-btn class="Btn"><p>Search</p></v-btn>
    </div>
    <v-row class="body_row">
      <div class="col-12 headerSide">
        <div
          class="d-flex align-items-center justify-space-between filterTitle"
        >
          <header v-if="type == 'off-plan'">
            Off-plan properties for sale in UAE
          </header>
          <header v-else>Properties for sale in UAE</header>
          <span>Clear all filters</span>
        </div>
        <p class="result">1,233 results</p>
      </div>
      <div
        data-aos="fade-up"
        data-aos-duration="400"
        class="col-12 col-sm-6 col-md-4 col-lg-4 col-xl-3 propcols"
        v-for="(items, index) in 9"
        :key="index"
      >
        <property-card :property="properties[0]"></property-card>
      </div>
      <div class="text-center col-12 mb-5">
        <v-pagination
          color="var(--primary-color)"
          v-model="page"
          :length="10"
          :total-visible="5"
          circle
        ></v-pagination>
      </div> </v-row
  ></v-container>
</template>

<script>
export default {
  props: ["type"],
  data() {
    return {
      page: 1,
      tab: null,
      close_on_content_click: false,
      propsbox: false,
      bedsbox: false,
      pricesbox: false,
      min_width: 325,
      nudge_bottom: 10,
      nudge_left: "70%",
      bednbath: "125%",
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
  mounted() {
    var nx = window.innerWidth;
    if (nx < 1264) {
      this.bednbath = "0";
      this.nudge_left = "0";
    }
    window.addEventListener("resize", function (event) {
      var w = window.innerWidth;
      nx = w;
    });
    $(window).resize(() => {
      if (nx <= 1264) {
        this.bednbath = "0";
        this.nudge_left = "0";
      } else {
        this.bednbath = "125%";
        this.nudge_left = "75%";
      }
    });
  },
  methods: {
    showModal(type) {
      switch (type) {
        case "filter":
          this.$refs.filterModal.showFilterModal();
          break;
        default:
          break;
      }
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
.filterContainer {
  padding-top: 71px;
  animation: transIn 0.8s linear 0s;
  .headerSide {
    padding: 12px 24px 0;
  }
  .filterTitle {
    header {
      font-weight: 600;
      font-size: 2.4rem;
      color: var(--secondary-color);
    }
    span {
      font-weight: 600;
      font-size: 1.6rem;
      color: var(--property-subtext-color);
      cursor: pointer;
      display: none;
    }
  }
  p.result {
    font-weight: 600;
    font-size: 1.8rem;
    color: var(--property-subtext-color);
    margin-bottom: 0;
  }
}
.search_grid {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  row-gap: 17px;
  column-gap: 30px;
  margin-bottom: 32px;
  padding: 12px;
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
.noShow {
  display: none !important;
}
// search list styles
.v-menu__content.theme--light.menuable__content__active:has(.searchList) {
  border-radius: 0;
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
    cursor: pointer;
    &.tabItem {
      animation: transIn 0.2s linear 0s;
    }
  }
  &.proptype {
    .gridMenu {
      .gridItem {
        animation: transIn 0.2s linear 0s;
      }
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
  input {
    padding: 0 10px;
    width: 100%;
    background-color: transparent;
    font-size: 1.4rem;
    height: 4.9rem;
    font-size: 1.8rem;
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
      width: 160px;
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
::-webkit-scrollbar {
  width: 5px !important;
  height: 5px !important;
}

/* Track */
::-webkit-scrollbar-track {
  box-shadow: none;
  border-radius: 10px;
  background: var(--border05-color);
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
@media (max-width: 1263px) {
  .search_grid {
    grid-template-columns: repeat(3, 1fr) !important;
    .Btn {
      grid-column: span 1 !important;
    }
  }
}
@media (max-width: 768px) {
  .headerSide {
    padding: 12px 12px 0 !important;
  }
}
@media (min-width: 600px) {
  .filterTitle {
    span {
      display: block !important;
    }
  }
}
@media (max-width: 599px) {
  .filterTitle {
    header {
      font-size: 1.8rem !important;
    }
  }
  p.result {
    font-weight: 1.6rem !important;
  }
  .search_grid {
    column-gap: 17px !important;
    row-gap: 15px !important;
    .dropdown.mobile {
      display: none !important;
    }
    .dropdown {
      padding: 0 15px 0 5px !important;
      span {
        font-size: 1.4rem !important;
      }
      svg path {
        fill: var(--primary-color);
        stroke: var(--primary-color);
      }
      svg circle {
        stroke: var(--primary-color);
      }
    }
    .Btn {
      grid-column: span 2 !important;
      p {
        font-size: 1.6rem !important;
      }
    }
  }
  .noShow {
    display: flex !important;
  }
}
</style>