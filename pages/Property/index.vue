<template>
  <section id="property-view">
    <v-container class="property-view">
      <v-row class="body_row">
        <!-- back nav  -->
        <div class="col-12">
          <div onclick="history.back()" class="backLink">
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M9 12L8.64645 11.6464L8.29289 12L8.64645 12.3536L9 12ZM14.6464 5.64645L8.64645 11.6464L9.35355 12.3536L15.3536 6.35355L14.6464 5.64645ZM8.64645 12.3536L14.6464 18.3536L15.3536 17.6464L9.35355 11.6464L8.64645 12.3536Z"
                fill="#BF9001"
              />
            </svg>
            <p>Back</p>
          </div>
        </div>
        <!-- header and property subtext  -->
        <div class="col-12 col-md-4 col-lg-4 col-xl-4">
          <header class="header_left">
            Apartment for sale in imperial avenue, downtown dubai
          </header>
          <p class="header_subtext">Imperial Avenue, Dubai, Downtown Dubai</p>
        </div>
        <!-- property actions  -->
        <div class="col-12 col-md-8 col-lg-8 col-xl-8">
          <div class="propertyActionWrapper">
            <v-btn class="Btn">
              <svg
                width="17"
                height="17"
                viewBox="0 0 17 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M4.25 10.625C5.42361 10.625 6.375 9.67361 6.375 8.5C6.375 7.32639 5.42361 6.375 4.25 6.375C3.07639 6.375 2.125 7.32639 2.125 8.5C2.125 9.67361 3.07639 10.625 4.25 10.625Z"
                  stroke="#BF9001"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M11.6875 15.4062C12.8611 15.4062 13.8125 14.4549 13.8125 13.2812C13.8125 12.1076 12.8611 11.1562 11.6875 11.1562C10.5139 11.1562 9.5625 12.1076 9.5625 13.2812C9.5625 14.4549 10.5139 15.4062 11.6875 15.4062Z"
                  stroke="#BF9001"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M11.6875 5.84375C12.8611 5.84375 13.8125 4.89236 13.8125 3.71875C13.8125 2.54514 12.8611 1.59375 11.6875 1.59375C10.5139 1.59375 9.5625 2.54514 9.5625 3.71875C9.5625 4.89236 10.5139 5.84375 11.6875 5.84375Z"
                  stroke="#BF9001"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M9.90195 4.86768L6.03711 7.35127"
                  stroke="#BF9001"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M6.03711 9.64893L9.90195 12.1325"
                  stroke="#BF9001"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <span>Share</span>
            </v-btn>
            <v-btn class="Btn">
              <svg
                width="17"
                height="17"
                viewBox="0 0 17 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M3.15321 9.85157L8.07798 14.4779L8.07799 14.4779C8.15309 14.5484 8.19065 14.5837 8.22782 14.6079C8.39367 14.7159 8.60763 14.7159 8.77349 14.6079C8.81065 14.5837 8.8482 14.5484 8.9233 14.4779L8.92332 14.4779L13.8481 9.85157C15.2337 8.54992 15.402 6.40793 14.2366 4.90588L14.0175 4.62345C12.6233 2.82658 9.82497 3.12793 8.84537 5.18042C8.707 5.47035 8.2943 5.47035 8.15593 5.18042C7.17633 3.12793 4.37796 2.82658 2.98383 4.62345L2.7647 4.90588C1.59932 6.40793 1.76759 8.54992 3.15321 9.85157Z"
                  stroke="#BF9001"
                />
              </svg>
              <span>Favorite</span>
            </v-btn>
            <v-btn class="Btn">
              <svg
                width="17"
                height="17"
                viewBox="0 0 17 17"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <circle
                  cx="7.79232"
                  cy="7.79159"
                  r="4.95833"
                  stroke="#BF9001"
                  stroke-width="2"
                />
                <path
                  d="M14.166 14.1667L12.041 12.0417"
                  stroke="#BF9001"
                  stroke-width="2"
                  stroke-linecap="round"
                />
              </svg>

              <span>Browse nearby listings</span>
            </v-btn>
          </div>
        </div>
        <!-- property large img  -->
        <div class="col-12 col-md-8 col-lg-8 col-xl-8 PropImgWrapper lg">
          <!-- <img src=./images/pngs/largeProp.png" alt="" /> -->
          <iframe
            src="https://www.youtube.com/embed/kdZYhfHYHtY?rel=0&showinfo=0&autohide=1&modestbranding=1"
            title="YouTube video player"
            frameborder="0"
            style="border: 0; background: transparent"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <!-- property small img  -->
        <v-row class="col-12 col-md-4 col-lg-4 col-xl-4 PropImgWrapper srow">
          <div class="col-6 col-md-12 col-lg-12 col-xl-12 smallPropImgWrapper">
            <img @click="showModal" src=./images/pngs/smallProp01.png" alt="" />
          </div>
          <div
            class="
              col-6 col-md-12 col-lg-12 col-xl-12
              smallPropImgWrapper
              box-2
              relative
            "
          >
            <img @click="showModal" src=./images/pngs/smallProp02.png" alt="" />
            <v-btn @click="showModal" class="Btn viewMore">
              <svg
                width="24"
                height="24"
                viewBox="0 0 24 24"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M3 11C3 7.22876 3 5.34315 4.17157 4.17157C5.34315 3 7.22876 3 11 3H13C16.7712 3 18.6569 3 19.8284 4.17157C21 5.34315 21 7.22876 21 11V13C21 16.7712 21 18.6569 19.8284 19.8284C18.6569 21 16.7712 21 13 21H11C7.22876 21 5.34315 21 4.17157 19.8284C3 18.6569 3 16.7712 3 13V11Z"
                  stroke="#BF9001"
                />
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M18.9976 14.2904L18.6544 13.9471L18.6385 13.9313C18.238 13.5307 17.9149 13.2077 17.6314 12.9687C17.3394 12.7226 17.055 12.5353 16.7221 12.4349C16.2512 12.2928 15.7488 12.2928 15.2779 12.4349C14.945 12.5353 14.6606 12.7226 14.3686 12.9687C14.0851 13.2077 13.762 13.5307 13.3615 13.9313L13.3456 13.9471C13.0459 14.2469 12.8458 14.4462 12.6832 14.5807C12.5218 14.7142 12.452 14.7359 12.4237 14.7408C12.3029 14.762 12.1785 14.7381 12.0742 14.6735C12.0498 14.6584 11.993 14.6123 11.8928 14.4285C11.7917 14.2432 11.68 13.9838 11.513 13.5942L11.4596 13.4696L11.4475 13.4414L11.4475 13.4414C11.0829 12.5907 10.7931 11.9144 10.5107 11.4126C10.2237 10.9026 9.90522 10.4984 9.44575 10.268C9.03426 10.0618 8.57382 9.97308 8.11515 10.0118C7.603 10.055 7.15716 10.3121 6.70134 10.6789C6.25273 11.04 5.73245 11.5603 5.07798 12.2148L5.07798 12.2148L5.05634 12.2364L5 12.2928V12.9999C5 13.2462 5.00007 13.4816 5.00044 13.7065L5.76344 12.9435C6.44443 12.2626 6.92686 11.7811 7.32835 11.458C7.72756 11.1366 7.98255 11.0265 8.19924 11.0082C8.47444 10.985 8.75071 11.0382 8.9976 11.162C9.192 11.2594 9.38786 11.4564 9.63918 11.903C9.89194 12.3521 10.1611 12.9783 10.5404 13.8635L10.5938 13.9881L10.6034 14.0105L10.6034 14.0105C10.7583 14.3719 10.8884 14.6754 11.0149 14.9073C11.1448 15.1455 11.3038 15.3727 11.5479 15.5238C11.8608 15.7175 12.2341 15.7894 12.5966 15.7258C12.8794 15.6761 13.1114 15.5242 13.3204 15.3513C13.524 15.183 13.7575 14.9495 14.0355 14.6714L14.0527 14.6542C14.4728 14.2341 14.766 13.9416 15.013 13.7334C15.2553 13.5292 15.4185 13.437 15.5667 13.3922C15.8493 13.307 16.1507 13.307 16.4333 13.3922C16.5815 13.437 16.7447 13.5292 16.987 13.7334C17.234 13.9416 17.5272 14.2341 17.9473 14.6542L18.9755 15.6825C18.9887 15.2721 18.9948 14.812 18.9976 14.2904Z"
                  fill="#BF9001"
                />
                <circle cx="16.5" cy="7.5" r="1.5" fill="#BF9001" />
              </svg>
              <span>View all images</span>
            </v-btn>
          </div>
        </v-row>
        <!-- features col  -->
        <div
          class="col-12 col-md-8 col-lg-8 col-xl-8 featuresWrapper"
          style="margin-top: 20px; margin-bottom: 29px; padding-bottom: 0"
        >
          <div class="features">
            <aside>
              <p>Bedrooms</p>
              <div>
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M19 7H5V14H3V5H1V20H3V17H21V20H23V11C23 9.93913 22.5786 8.92172 21.8284 8.17157C21.0783 7.42143 20.0609 7 19 7Z"
                    fill="#6D7175"
                  />
                </svg>

                <span>3</span>
              </div>
            </aside>
            <aside>
              <p>Bathrooms</p>
              <div>
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M21.75 13.125H3.75V4.6875C3.74913 4.36975 3.81129 4.05498 3.9329 3.76142C4.0545 3.46786 4.23312 3.20133 4.45842 2.97726L4.47717 2.95852C4.83026 2.60594 5.2836 2.37098 5.77524 2.28572C6.26688 2.20046 6.77286 2.26907 7.22405 2.48217C6.79794 3.19064 6.62083 4.02119 6.72086 4.84185C6.82089 5.66251 7.19233 6.4262 7.77614 7.01156L8.28947 7.52489L7.34461 8.4698L8.4052 9.53039L9.35006 8.58553L14.5855 3.3502L15.5303 2.40534L14.4697 1.3447L13.5248 2.28956L13.0115 1.77623C12.3969 1.16336 11.5867 0.785558 10.7222 0.708671C9.85764 0.631784 8.99353 0.860685 8.28042 1.35548C7.52846 0.8806 6.63734 0.675589 5.75346 0.774129C4.86958 0.87267 4.04549 1.2689 3.41658 1.89773L3.39783 1.91648C3.03279 2.27953 2.74338 2.71137 2.54635 3.18702C2.34933 3.66266 2.2486 4.17266 2.25 4.6875V13.125H0.75V14.625H2.25V16.0641C2.24997 16.185 2.26947 16.3051 2.30775 16.4198L3.70312 20.6057C3.77759 20.8298 3.92078 21.0248 4.11235 21.1629C4.30392 21.301 4.53413 21.3752 4.77028 21.375H5.37497L4.82812 23.25H6.39061L6.9375 21.375H16.6922L17.2547 23.25H18.8203L18.2578 21.375H19.2295C19.4657 21.3752 19.696 21.301 19.8876 21.1629C20.0792 21.0248 20.2224 20.8299 20.2969 20.6057L21.6922 16.4198C21.7304 16.3051 21.75 16.185 21.75 16.0641V14.625H23.25V13.125H21.75Z"
                    fill="#6D7175"
                  />
                </svg>

                <span>2</span>
              </div>
            </aside>
            <aside>
              <p>Square Area</p>
              <div>
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M15 15V14H14V15H15ZM20.2929 21.7071C20.6834 22.0976 21.3166 22.0976 21.7071 21.7071C22.0976 21.3166 22.0976 20.6834 21.7071 20.2929L20.2929 21.7071ZM15 9H14V10H15V9ZM21.7071 3.70711C22.0976 3.31658 22.0976 2.68342 21.7071 2.29289C21.3166 1.90237 20.6834 1.90237 20.2929 2.29289L21.7071 3.70711ZM9 15H10V14H9V15ZM2.29289 20.2929C1.90237 20.6834 1.90237 21.3166 2.29289 21.7071C2.68342 22.0976 3.31658 22.0976 3.70711 21.7071L2.29289 20.2929ZM9 9V10H10V9H9ZM3.70711 2.29289C3.31658 1.90237 2.68342 1.90237 2.29289 2.29289C1.90237 2.68342 1.90237 3.31658 2.29289 3.70711L3.70711 2.29289ZM16 20V15H14V20H16ZM15 16H20V14H15V16ZM14.2929 15.7071L20.2929 21.7071L21.7071 20.2929L15.7071 14.2929L14.2929 15.7071ZM14 4V9H16V4H14ZM15 10H20V8H15V10ZM15.7071 9.70711L21.7071 3.70711L20.2929 2.29289L14.2929 8.29289L15.7071 9.70711ZM10 20V15H8V20H10ZM9 14H4V16H9V14ZM8.29289 14.2929L2.29289 20.2929L3.70711 21.7071L9.70711 15.7071L8.29289 14.2929ZM8 4V9H10V4H8ZM9 8H4V10H9V8ZM9.70711 8.29289L3.70711 2.29289L2.29289 3.70711L8.29289 9.70711L9.70711 8.29289Z"
                    fill="#6D7175"
                  />
                </svg>

                <span>936</span>
              </div>
            </aside>
          </div>
        </div>
        <!-- contact row  -->
        <v-row
          class="col-12 col-md-4 col-lg-4 col-xl-4 contact_wrapper"
          style="margin-top: 20px; margin-bottom: 29px"
        >
          <!-- call phone  -->
          <div class="col-6 col-md-12 col-lg-12 col-xl-12 contactCol">
            <a href="tel:+971586276573">
              <v-btn class="Btn contact phone">
                <svg
                  width="35"
                  height="36"
                  viewBox="0 0 35 36"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle
                    cx="17.1818"
                    cy="18.0002"
                    r="17.1818"
                    fill="#BF9001"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M12.2568 11.9676C12.5418 11.6829 12.9353 11.5343 13.3374 11.5594C13.7394 11.5845 14.1114 11.7809 14.3588 12.0988L15.8045 13.9562C16.0694 14.2969 16.1628 14.7407 16.0581 15.1595L15.6176 16.9234C15.5713 17.1092 15.6257 17.3057 15.761 17.4413L17.7398 19.4202C17.8755 19.5558 18.0724 19.6102 18.2584 19.5636L20.0214 19.123C20.4401 19.0183 20.8838 19.1119 21.2246 19.3767L23.0818 20.8217C23.7495 21.3412 23.8107 22.3279 23.2131 22.9247L22.3803 23.7575C21.7843 24.3535 20.8936 24.6153 20.0633 24.3229C17.938 23.5751 16.0084 22.3583 14.4176 20.7629C12.8224 19.1722 11.6057 17.2427 10.8579 15.1176C10.5663 14.288 10.8281 13.3964 11.424 12.8004L12.2568 11.9676Z"
                    fill="white"
                  />
                </svg>
                <span class="hidden">Call (+971) 586 276573</span>
                <span class="visible">+971 586 276573</span>
              </v-btn>
            </a>
          </div>
          <!-- contact whatsapp  -->
          <div class="col-6 col-md-12 col-lg-12 col-xl-12 contactCol">
            <a href="">
              <v-btn class="Btn contact whatsapp">
                <svg
                  width="35"
                  height="35"
                  viewBox="0 0 35 35"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle
                    cx="17.1818"
                    cy="17.1818"
                    r="17.1818"
                    fill="#25D366"
                  />
                  <path
                    d="M23.2565 10.5211C21.6666 8.92734 19.5492 8.05078 17.2989 8.05078C12.6543 8.05078 8.87483 11.8302 8.87483 16.4749C8.87483 17.9586 9.26189 19.4081 9.99805 20.6869L8.80273 25.0508L13.269 23.8782C14.4985 24.5499 15.8835 24.9028 17.2951 24.9028H17.2989C21.9398 24.9028 25.8027 21.1233 25.8027 16.4787C25.8027 14.2285 24.8465 12.1148 23.2565 10.5211ZM17.2989 23.4836C16.0391 23.4836 14.8059 23.1459 13.732 22.5084L13.4777 22.3566L10.8291 23.051L11.5349 20.4669L11.3679 20.2012C10.6659 19.0856 10.2978 17.7992 10.2978 16.4749C10.2978 12.6157 13.4398 9.47377 17.3027 9.47377C19.1735 9.47377 20.9304 10.2023 22.2509 11.5267C23.5715 12.851 24.3835 14.6079 24.3797 16.4787C24.3797 20.3416 21.1581 23.4836 17.2989 23.4836ZM21.1391 18.2394C20.9304 18.1331 19.8945 17.6247 19.7009 17.5564C19.5074 17.4843 19.367 17.4501 19.2266 17.6626C19.0862 17.8751 18.684 18.3456 18.5588 18.4898C18.4373 18.6302 18.3121 18.6492 18.1034 18.543C16.8664 17.9244 16.0543 17.4387 15.2384 16.0385C15.0222 15.6666 15.4547 15.6932 15.857 14.8887C15.9253 14.7483 15.8911 14.6269 15.838 14.5206C15.7849 14.4144 15.3637 13.3785 15.1891 12.9573C15.0184 12.5474 14.8438 12.6044 14.7148 12.5968C14.5934 12.5892 14.453 12.5892 14.3126 12.5892C14.1722 12.5892 13.9445 12.6423 13.7509 12.851C13.5574 13.0635 13.0148 13.572 13.0148 14.6079C13.0148 15.6439 13.7699 16.6456 13.8724 16.786C13.9786 16.9265 15.3561 19.0515 17.4697 19.966C18.8054 20.5427 19.3291 20.5921 19.9969 20.4934C20.403 20.4327 21.2416 19.9849 21.4161 19.4916C21.5907 18.9983 21.5907 18.5771 21.5376 18.4898C21.4882 18.395 21.3478 18.3419 21.1391 18.2394Z"
                    fill="white"
                  />
                </svg>
                <span class="hidden">Send a WhatsApp message</span>
                <span class="visible">Whatsapp</span>
              </v-btn>
            </a>
          </div>
        </v-row>
        <!-- application form mobile -->
        <!-- fix implementation  -->
        <div
          class="col-12 col-md-4 col-lg-4 col-xl-4"
          style="padding-left: 0; margin-bottom: 24px"
        >
          <v-card class="authCard m3x10 mobile">
            <div class="modal_content">
              <form action="" class="content_area">
                <span
                  class="subtext"
                  style="
                    font-weight: 400;
                    font-size: 1.8rem;
                    color: var(--property-subtext-color);
                  "
                  >Sell Price</span
                >
                <header
                  class="text-left"
                  style="
                    margin-bottom: 23px;
                    margin-top: 5px;
                    color: var(--primary-color);
                  "
                >
                  AED 5,700,000
                </header>
                <v-row class="row_form">
                  <div class="relative col-12">
                    <input
                      id="fname"
                      required
                      autocomplete="off"
                      type="text"
                      name=""
                      v-model="contact.name"
                    />
                    <label
                      for="fname"
                      :class="{ containsElement: contact.name }"
                      class="placeholder"
                      >Name <span class="text-danger">*</span></label
                    >
                  </div>
                  <div class="relative col-12">
                    <input
                      id="email"
                      required
                      autocomplete="off"
                      type="email"
                      name=""
                      v-model="contact.email"
                    />
                    <label
                      for="email"
                      :class="{ containsElement: contact.email }"
                      class="placeholder"
                      >Email <span class="text-danger">*</span></label
                    >
                  </div>
                  <div class="relative col-12">
                    <input
                      id="phone"
                      required
                      autocomplete="off"
                      type="text"
                      name=""
                      v-model="contact.phone"
                    />
                    <label
                      for="phone"
                      :class="{ containsElement: contact.phone }"
                      class="placeholder"
                      >Phone <span class="text-danger">*</span></label
                    >
                  </div>
                  <div class="relative col-12">
                    <textarea
                      required
                      rows="5"
                      v-model="contact.message"
                      placeholder="Message *"
                      cols=""
                    ></textarea>
                  </div>
                </v-row>
                <footer class="footer">
                  <v-btn class="Btn ctaBtn"
                    ><svg
                      width="20"
                      height="21"
                      viewBox="0 0 20 21"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M7.08398 10.9165L12.9173 10.9165"
                        stroke="white"
                        stroke-linecap="round"
                      />
                      <path
                        d="M7.08398 13.4165L10.4173 13.4165"
                        stroke="white"
                        stroke-linecap="round"
                      />
                      <path
                        d="M4.58398 5.81651C4.58398 4.97643 4.58398 4.55639 4.74747 4.23552C4.89128 3.95328 5.12076 3.7238 5.403 3.57999C5.72387 3.4165 6.14391 3.4165 6.98398 3.4165H10.2565C10.6234 3.4165 10.8069 3.4165 10.9795 3.45795C11.1326 3.49469 11.2789 3.5553 11.4131 3.63754C11.5645 3.73031 11.6942 3.86002 11.9536 4.11945L14.7144 6.88023C14.9738 7.13965 15.1035 7.26937 15.1963 7.42074C15.2785 7.55495 15.3391 7.70127 15.3759 7.85432C15.4173 8.02695 15.4173 8.2104 15.4173 8.57728V15.1832C15.4173 16.0232 15.4173 16.4433 15.2538 16.7642C15.11 17.0464 14.8805 17.2759 14.5983 17.4197C14.2774 17.5832 13.8574 17.5832 13.0173 17.5832H6.98398C6.14391 17.5832 5.72387 17.5832 5.403 17.4197C5.12076 17.2759 4.89128 17.0464 4.74747 16.7642C4.58398 16.4433 4.58398 16.0232 4.58398 15.1832V5.81651Z"
                        stroke="white"
                      />
                      <path
                        d="M10.416 3.4165V6.0165C10.416 6.85658 10.416 7.27662 10.5795 7.59749C10.7233 7.87973 10.9528 8.1092 11.235 8.25301C11.5559 8.4165 11.9759 8.4165 12.816 8.4165H15.416"
                        stroke="white"
                      />
                    </svg>
                    Apply Now</v-btn
                  >
                </footer>
              </form>
            </div>
          </v-card>
        </div>
        <!-- property info  -->
        <v-row class="col-12 col-md-8 col-lg-8 col-xl-8 about m3x0">
          <!-- about  -->
          <div class="col-12">
            <header style="margin-bottom: 17px">About this home</header>
            <span class="subtext"
              >Three Bedroom + maids for sale, in the Brand New tower to be
              handed over in December 2023, Imperial Avenue, in the heart of
              Downtown. This tower will have a modern contemporary finish like
              no other in Downtown. The apartment offers an en suite with every
              bedroom and Burj Khalifa Views from the balcony, living area and
              bedrooms. Call today to find out more.
            </span>
          </div>
          <!-- prop info  -->
          <v-row class="col-12">
            <div class="col-12">
              <header>Property Information</header>
            </div>
            <div class="col-12 col-md-6 col-lg-6 col-xl-6 propInfo">
              <table>
                <tbody>
                  <tr>
                    <td><span class="subtext">Status</span></td>
                    <td class="text-right">
                      <span class="propData">Completed</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Data Available</span></td>
                    <td class="text-right">
                      <span class="propData">Available now</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Type</span></td>
                    <td class="text-right">
                      <span class="propData">Home</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Laundry</span></td>
                    <td class="text-right">
                      <span class="propData">In Unit</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Cooling</span></td>
                    <td class="text-right">
                      <span class="propData">Air Conditioner</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Heating</span></td>
                    <td class="text-right">
                      <span class="propData">Forced Air</span>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
            <div class="col-12 col-md-6 col-lg-6 col-xl-6 propInfo">
              <table>
                <tbody>
                  <tr>
                    <td><span class="subtext">City</span></td>
                    <td class="text-right">
                      <span class="propData">Dubai</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Year Built</span></td>
                    <td class="text-right">
                      <span class="propData">2018</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Size</span></td>
                    <td class="text-right">
                      <span class="propData">936 sqft</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Lot Size</span></td>
                    <td class="text-right">
                      <span class="propData">2,173 sqft</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Parking Area</span></td>
                    <td class="text-right">
                      <span class="propData">Yes</span>
                    </td>
                  </tr>
                  <tr>
                    <td><span class="subtext">Deposit & Fees</span></td>
                    <td class="text-right">
                      <span class="propData">AED 5,700,000</span>
                    </td>
                  </tr>
                </tbody>
              </table>
            </div>
          </v-row>
          <!-- amenties  -->
          <v-row class="col-12">
            <div class="col-12">
              <header>Amenties</header>
            </div>
            <div class="col-12 col-md-4 col-lg-4 col-xl-4 amenties">
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Pets Allowed</span
                >
              </div>
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Free Wifi</span
                >
              </div>
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Private Pool</span
                >
              </div>
            </div>
            <div class="col-12 col-md-4 col-lg-4 col-xl-4 amenties">
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Private Gym</span
                >
              </div>
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Laundry Room</span
                >
              </div>
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Balcony or Terrace</span
                >
              </div>
            </div>
            <div class="col-12 col-md-4 col-lg-4 col-xl-4 amenties">
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Basement Parking</span
                >
              </div>
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Walk in Closet</span
                >
              </div>
              <div class="amenties_wrapper">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="12" cy="12" r="9" stroke="#BF9001" />
                  <path d="M8 12L11 15L16 9" stroke="#BF9001" />
                </svg>
                <span class="subtext" style="margin-bottom: -5px"
                  >Built In Wardrobes</span
                >
              </div>
            </div>
          </v-row>
          <!-- policy  -->
          <!-- <div class="col-12">
            <span class="subtext">
              You agree to sena homes terms of use & Privacy Policy. By choosing
              to contact a property.
            </span>
          </div> -->
          <!-- map  -->
          <div class="col-12">
            <header>
              Find this property in Imperial Avenue, Downtown Dubai
            </header>
            <!-- <div class="locationSpace"></div> -->
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m26!1m12!1m3!1d149960.3102064339!2d7.4595136578476975!3d9.003493053299069!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!4m11!3e6!4m3!3m2!1d8.9485393!2d7.5509243999999995!4m5!1s0x104e0b4fd7908607%3A0x32c56f1f38f4f640!2sbex%20it!3m2!1d9.088953!2d7.4956325999999995!5e0!3m2!1sen!2sng!4v1670342725623!5m2!1sen!2sng"
              height="450"
              style="border: 0"
              allowfullscreen=""
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"
            ></iframe>
          </div>
        </v-row>
        <!-- application form desktop -->
        <!-- fix implementation  -->
        <div
          class="col-12 col-md-4 col-lg-4 col-xl-4"
          style="padding-left: 0; margin-top: 24px"
        >
          <v-card class="authCard m3x10 desktop">
            <div class="modal_content">
              <form action="" class="content_area">
                <span
                  class="subtext"
                  style="
                    font-weight: 400;
                    font-size: 1.8rem;
                    color: var(--property-subtext-color);
                  "
                  >Sell Price</span
                >
                <header
                  class="text-left"
                  style="
                    margin-bottom: 23px;
                    margin-top: 5px;
                    color: var(--primary-color);
                  "
                >
                  AED 5,700,000
                </header>
                <v-row class="row_form">
                  <div class="relative col-12">
                    <input
                      id="fname"
                      required
                      autocomplete="off"
                      type="text"
                      name=""
                      v-model="contact.name"
                    />
                    <label
                      for="fname"
                      :class="{ containsElement: contact.name }"
                      class="placeholder"
                      >Name <span class="text-danger">*</span></label
                    >
                  </div>
                  <div class="relative col-12">
                    <input
                      id="email"
                      required
                      autocomplete="off"
                      type="email"
                      name=""
                      v-model="contact.email"
                    />
                    <label
                      for="email"
                      :class="{ containsElement: contact.email }"
                      class="placeholder"
                      >Email <span class="text-danger">*</span></label
                    >
                  </div>
                  <div class="relative col-12">
                    <input
                      id="phone"
                      required
                      autocomplete="off"
                      type="text"
                      name=""
                      v-model="contact.phone"
                    />
                    <label
                      for="phone"
                      :class="{ containsElement: contact.phone }"
                      class="placeholder"
                      >Phone <span class="text-danger">*</span></label
                    >
                  </div>
                  <div class="relative col-12">
                    <textarea
                      required
                      rows="5"
                      v-model="contact.message"
                      placeholder="Message *"
                      cols=""
                    ></textarea>
                  </div>
                </v-row>
                <footer class="footer">
                  <v-btn class="Btn"
                    ><svg
                      width="20"
                      height="21"
                      viewBox="0 0 20 21"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M7.08398 10.9165L12.9173 10.9165"
                        stroke="white"
                        stroke-linecap="round"
                      />
                      <path
                        d="M7.08398 13.4165L10.4173 13.4165"
                        stroke="white"
                        stroke-linecap="round"
                      />
                      <path
                        d="M4.58398 5.81651C4.58398 4.97643 4.58398 4.55639 4.74747 4.23552C4.89128 3.95328 5.12076 3.7238 5.403 3.57999C5.72387 3.4165 6.14391 3.4165 6.98398 3.4165H10.2565C10.6234 3.4165 10.8069 3.4165 10.9795 3.45795C11.1326 3.49469 11.2789 3.5553 11.4131 3.63754C11.5645 3.73031 11.6942 3.86002 11.9536 4.11945L14.7144 6.88023C14.9738 7.13965 15.1035 7.26937 15.1963 7.42074C15.2785 7.55495 15.3391 7.70127 15.3759 7.85432C15.4173 8.02695 15.4173 8.2104 15.4173 8.57728V15.1832C15.4173 16.0232 15.4173 16.4433 15.2538 16.7642C15.11 17.0464 14.8805 17.2759 14.5983 17.4197C14.2774 17.5832 13.8574 17.5832 13.0173 17.5832H6.98398C6.14391 17.5832 5.72387 17.5832 5.403 17.4197C5.12076 17.2759 4.89128 17.0464 4.74747 16.7642C4.58398 16.4433 4.58398 16.0232 4.58398 15.1832V5.81651Z"
                        stroke="white"
                      />
                      <path
                        d="M10.416 3.4165V6.0165C10.416 6.85658 10.416 7.27662 10.5795 7.59749C10.7233 7.87973 10.9528 8.1092 11.235 8.25301C11.5559 8.4165 11.9759 8.4165 12.816 8.4165H15.416"
                        stroke="white"
                      />
                    </svg>
                    Apply Now</v-btn
                  >
                </footer>
              </form>
            </div>
          </v-card>
        </div>
        <!-- ratings  -->
        <div class="col-12 col-md-8 col-lg-8 col-xl-8 m3x0">
          <form>
            <div
              class="d-flex align-items-center justify-space-between"
              style="margin-bottom: 30px"
            >
              <header>Reviews & Ratings</header>
              <v-btn type="submit" class="Btn reviewPost lg"
                ><span>Post</span></v-btn
              >
            </div>
            <p class="ratings">Write your review</p>
            <textarea required rows="5" cols=""></textarea>
            <div style="margin-bottom: 31px" class="text-right">
              <span class="propData">0 / 250</span>
            </div>
            <p class="ratings">Rate this property</p>
            <v-card class="ratings_card">
              <div>
                <svg
                  width="38"
                  height="38"
                  viewBox="0 0 38 38"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M16.0619 10.4938C17.3073 7.38888 17.9301 5.83643 19.0009 5.83643C20.0718 5.83643 20.6945 7.38888 21.94 10.4938L21.998 10.6384C22.7016 12.3925 23.0534 13.2696 23.7704 13.8027C24.4874 14.3357 25.4286 14.42 27.3111 14.5886L27.6514 14.6191C30.7323 14.895 32.2727 15.033 32.6023 16.013C32.9319 16.9931 31.7879 18.0339 29.5 20.1155L28.7364 20.8102C27.5781 21.8639 26.999 22.3908 26.7291 23.0813C26.6788 23.2102 26.6369 23.3421 26.6038 23.4764C26.4264 24.1963 26.596 24.9606 26.9351 26.4893L27.0407 26.9651C27.664 29.7745 27.9757 31.1792 27.4315 31.785C27.2282 32.0114 26.9639 32.1745 26.6703 32.2546C25.8847 32.4689 24.7693 31.56 22.5384 29.7422C21.0736 28.5486 20.3411 27.9517 19.5002 27.8175C19.1694 27.7647 18.8324 27.7647 18.5016 27.8175C17.6607 27.9517 16.9283 28.5486 15.4634 29.7422C13.2326 31.56 12.1172 32.4689 11.3315 32.2546C11.0379 32.1745 10.7737 32.0114 10.5703 31.785C10.0262 31.1792 10.3378 29.7745 10.9611 26.9651L11.0667 26.4893C11.4059 24.9606 11.5755 24.1963 11.398 23.4764C11.3649 23.3421 11.3231 23.2102 11.2727 23.0813C11.0028 22.3908 10.4237 21.8639 9.26549 20.8102L8.50188 20.1155C6.21389 18.0339 5.0699 16.9931 5.39952 16.013C5.72913 15.033 7.26957 14.895 10.3504 14.6191L10.6908 14.5886C12.5732 14.42 13.5144 14.3357 14.2314 13.8027C14.9485 13.2696 15.3003 12.3925 16.0039 10.6384L16.0619 10.4938Z"
                    stroke="#FFD841"
                  />
                </svg>
                <svg
                  width="38"
                  height="38"
                  viewBox="0 0 38 38"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M16.0619 10.4938C17.3073 7.38888 17.9301 5.83643 19.0009 5.83643C20.0718 5.83643 20.6945 7.38888 21.94 10.4938L21.998 10.6384C22.7016 12.3925 23.0534 13.2696 23.7704 13.8027C24.4874 14.3357 25.4286 14.42 27.3111 14.5886L27.6514 14.6191C30.7323 14.895 32.2727 15.033 32.6023 16.013C32.9319 16.9931 31.7879 18.0339 29.5 20.1155L28.7364 20.8102C27.5781 21.8639 26.999 22.3908 26.7291 23.0813C26.6788 23.2102 26.6369 23.3421 26.6038 23.4764C26.4264 24.1963 26.596 24.9606 26.9351 26.4893L27.0407 26.9651C27.664 29.7745 27.9757 31.1792 27.4315 31.785C27.2282 32.0114 26.9639 32.1745 26.6703 32.2546C25.8847 32.4689 24.7693 31.56 22.5384 29.7422C21.0736 28.5486 20.3411 27.9517 19.5002 27.8175C19.1694 27.7647 18.8324 27.7647 18.5016 27.8175C17.6607 27.9517 16.9283 28.5486 15.4634 29.7422C13.2326 31.56 12.1172 32.4689 11.3315 32.2546C11.0379 32.1745 10.7737 32.0114 10.5703 31.785C10.0262 31.1792 10.3378 29.7745 10.9611 26.9651L11.0667 26.4893C11.4059 24.9606 11.5755 24.1963 11.398 23.4764C11.3649 23.3421 11.3231 23.2102 11.2727 23.0813C11.0028 22.3908 10.4237 21.8639 9.26549 20.8102L8.50188 20.1155C6.21389 18.0339 5.0699 16.9931 5.39952 16.013C5.72913 15.033 7.26957 14.895 10.3504 14.6191L10.6908 14.5886C12.5732 14.42 13.5144 14.3357 14.2314 13.8027C14.9485 13.2696 15.3003 12.3925 16.0039 10.6384L16.0619 10.4938Z"
                    stroke="#FFD841"
                  />
                </svg>
                <svg
                  width="38"
                  height="38"
                  viewBox="0 0 38 38"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M16.0619 10.4938C17.3073 7.38888 17.9301 5.83643 19.0009 5.83643C20.0718 5.83643 20.6945 7.38888 21.94 10.4938L21.998 10.6384C22.7016 12.3925 23.0534 13.2696 23.7704 13.8027C24.4874 14.3357 25.4286 14.42 27.3111 14.5886L27.6514 14.6191C30.7323 14.895 32.2727 15.033 32.6023 16.013C32.9319 16.9931 31.7879 18.0339 29.5 20.1155L28.7364 20.8102C27.5781 21.8639 26.999 22.3908 26.7291 23.0813C26.6788 23.2102 26.6369 23.3421 26.6038 23.4764C26.4264 24.1963 26.596 24.9606 26.9351 26.4893L27.0407 26.9651C27.664 29.7745 27.9757 31.1792 27.4315 31.785C27.2282 32.0114 26.9639 32.1745 26.6703 32.2546C25.8847 32.4689 24.7693 31.56 22.5384 29.7422C21.0736 28.5486 20.3411 27.9517 19.5002 27.8175C19.1694 27.7647 18.8324 27.7647 18.5016 27.8175C17.6607 27.9517 16.9283 28.5486 15.4634 29.7422C13.2326 31.56 12.1172 32.4689 11.3315 32.2546C11.0379 32.1745 10.7737 32.0114 10.5703 31.785C10.0262 31.1792 10.3378 29.7745 10.9611 26.9651L11.0667 26.4893C11.4059 24.9606 11.5755 24.1963 11.398 23.4764C11.3649 23.3421 11.3231 23.2102 11.2727 23.0813C11.0028 22.3908 10.4237 21.8639 9.26549 20.8102L8.50188 20.1155C6.21389 18.0339 5.0699 16.9931 5.39952 16.013C5.72913 15.033 7.26957 14.895 10.3504 14.6191L10.6908 14.5886C12.5732 14.42 13.5144 14.3357 14.2314 13.8027C14.9485 13.2696 15.3003 12.3925 16.0039 10.6384L16.0619 10.4938Z"
                    stroke="#FFD841"
                  />
                </svg>
                <svg
                  width="38"
                  height="38"
                  viewBox="0 0 38 38"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M16.0619 10.4938C17.3073 7.38888 17.9301 5.83643 19.0009 5.83643C20.0718 5.83643 20.6945 7.38888 21.94 10.4938L21.998 10.6384C22.7016 12.3925 23.0534 13.2696 23.7704 13.8027C24.4874 14.3357 25.4286 14.42 27.3111 14.5886L27.6514 14.6191C30.7323 14.895 32.2727 15.033 32.6023 16.013C32.9319 16.9931 31.7879 18.0339 29.5 20.1155L28.7364 20.8102C27.5781 21.8639 26.999 22.3908 26.7291 23.0813C26.6788 23.2102 26.6369 23.3421 26.6038 23.4764C26.4264 24.1963 26.596 24.9606 26.9351 26.4893L27.0407 26.9651C27.664 29.7745 27.9757 31.1792 27.4315 31.785C27.2282 32.0114 26.9639 32.1745 26.6703 32.2546C25.8847 32.4689 24.7693 31.56 22.5384 29.7422C21.0736 28.5486 20.3411 27.9517 19.5002 27.8175C19.1694 27.7647 18.8324 27.7647 18.5016 27.8175C17.6607 27.9517 16.9283 28.5486 15.4634 29.7422C13.2326 31.56 12.1172 32.4689 11.3315 32.2546C11.0379 32.1745 10.7737 32.0114 10.5703 31.785C10.0262 31.1792 10.3378 29.7745 10.9611 26.9651L11.0667 26.4893C11.4059 24.9606 11.5755 24.1963 11.398 23.4764C11.3649 23.3421 11.3231 23.2102 11.2727 23.0813C11.0028 22.3908 10.4237 21.8639 9.26549 20.8102L8.50188 20.1155C6.21389 18.0339 5.0699 16.9931 5.39952 16.013C5.72913 15.033 7.26957 14.895 10.3504 14.6191L10.6908 14.5886C12.5732 14.42 13.5144 14.3357 14.2314 13.8027C14.9485 13.2696 15.3003 12.3925 16.0039 10.6384L16.0619 10.4938Z"
                    stroke="#FFD841"
                  />
                </svg>
                <svg
                  width="38"
                  height="38"
                  viewBox="0 0 38 38"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M16.0619 10.4938C17.3073 7.38888 17.9301 5.83643 19.0009 5.83643C20.0718 5.83643 20.6945 7.38888 21.94 10.4938L21.998 10.6384C22.7016 12.3925 23.0534 13.2696 23.7704 13.8027C24.4874 14.3357 25.4286 14.42 27.3111 14.5886L27.6514 14.6191C30.7323 14.895 32.2727 15.033 32.6023 16.013C32.9319 16.9931 31.7879 18.0339 29.5 20.1155L28.7364 20.8102C27.5781 21.8639 26.999 22.3908 26.7291 23.0813C26.6788 23.2102 26.6369 23.3421 26.6038 23.4764C26.4264 24.1963 26.596 24.9606 26.9351 26.4893L27.0407 26.9651C27.664 29.7745 27.9757 31.1792 27.4315 31.785C27.2282 32.0114 26.9639 32.1745 26.6703 32.2546C25.8847 32.4689 24.7693 31.56 22.5384 29.7422C21.0736 28.5486 20.3411 27.9517 19.5002 27.8175C19.1694 27.7647 18.8324 27.7647 18.5016 27.8175C17.6607 27.9517 16.9283 28.5486 15.4634 29.7422C13.2326 31.56 12.1172 32.4689 11.3315 32.2546C11.0379 32.1745 10.7737 32.0114 10.5703 31.785C10.0262 31.1792 10.3378 29.7745 10.9611 26.9651L11.0667 26.4893C11.4059 24.9606 11.5755 24.1963 11.398 23.4764C11.3649 23.3421 11.3231 23.2102 11.2727 23.0813C11.0028 22.3908 10.4237 21.8639 9.26549 20.8102L8.50188 20.1155C6.21389 18.0339 5.0699 16.9931 5.39952 16.013C5.72913 15.033 7.26957 14.895 10.3504 14.6191L10.6908 14.5886C12.5732 14.42 13.5144 14.3357 14.2314 13.8027C14.9485 13.2696 15.3003 12.3925 16.0039 10.6384L16.0619 10.4938Z"
                    stroke="#FFD841"
                  />
                </svg>
              </div>
            </v-card>
            <v-btn type="submit" class="Btn reviewPost sm"
              ><span>Post</span></v-btn
            >
            <span
              v-if="!showReview"
              @click="showReview = !showReview"
              class="subtext d-block"
              >0 Reviews & Ratings</span
            >
            <span
              v-else
              @click="showReview = !showReview"
              class="subtext d-block"
              >3 Reviews & Ratings</span
            >
            <div v-if="!showReview" class="no_reviews">
              <svg
                width="145"
                height="145"
                viewBox="0 0 145 145"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M29.2604 43.2699L26.5598 41.8939L26.5598 41.8939L29.2604 43.2699ZM31.8403 113.154L33.9835 115.298L33.9835 115.298L31.8403 113.154ZM108.277 98.0389L109.653 100.74L109.653 100.74L108.277 98.0389ZM116.224 90.0915L118.925 91.4675L118.925 91.4675L116.224 90.0915ZM116.224 43.2699L118.925 41.8939L118.925 41.8938L116.224 43.2699ZM108.277 35.3224L109.653 32.6219L109.653 32.6219L108.277 35.3224ZM37.2078 35.3224L35.8318 32.6219L35.8318 32.6219L37.2078 35.3224ZM43.1982 101.797L41.055 99.6533L43.1982 101.797ZM30.3093 62.4374C30.3093 57.2949 30.3116 53.6203 30.547 50.7399C30.7794 47.8948 31.224 46.0925 31.961 44.6459L26.5598 41.8939C25.3148 44.3374 24.7683 47.0263 24.5052 50.2463C24.245 53.4308 24.2474 57.3949 24.2474 62.4374H30.3093ZM30.3093 69.4304V62.4374H24.2474V69.4304H30.3093ZM24.1527 69.5252V99.6861H30.2145V69.5252H24.1527ZM24.1527 99.6861V111.226H30.2145V99.6861H24.1527ZM24.1527 111.226C24.1527 116.356 30.3557 118.925 33.9835 115.298L29.6971 111.011C29.7147 110.994 29.7788 110.949 29.8704 110.933C29.9454 110.92 29.9975 110.933 30.0274 110.946C30.0573 110.958 30.1033 110.986 30.1471 111.048C30.2007 111.124 30.2145 111.201 30.2145 111.226H24.1527ZM33.9835 115.298L45.3414 103.94L41.055 99.6533L29.6971 111.011L33.9835 115.298ZM89.1095 96.9901H47.4846V103.052H89.1095V96.9901ZM106.901 95.3383C105.454 96.0754 103.652 96.5199 100.807 96.7524C97.9266 96.9877 94.252 96.9901 89.1095 96.9901V103.052C94.152 103.052 98.1161 103.054 101.301 102.794C104.521 102.531 107.209 101.985 109.653 100.74L106.901 95.3383ZM113.524 88.7155C112.071 91.567 109.753 93.8854 106.901 95.3383L109.653 100.74C113.645 98.7054 116.891 95.4597 118.925 91.4675L113.524 88.7155ZM115.176 70.924C115.176 76.0665 115.173 79.741 114.938 82.6215C114.705 85.4665 114.261 87.2689 113.524 88.7155L118.925 91.4675C120.17 89.024 120.717 86.335 120.98 83.1151C121.24 79.9306 121.237 75.9664 121.237 70.924H115.176ZM115.176 62.4374V70.924H121.237V62.4374H115.176ZM113.524 44.6459C114.261 46.0925 114.705 47.8948 114.938 50.7399C115.173 53.6203 115.176 57.2949 115.176 62.4374H121.237C121.237 57.3949 121.24 53.4308 120.98 50.2463C120.717 47.0263 120.17 44.3374 118.925 41.8939L113.524 44.6459ZM106.901 38.023C109.753 39.476 112.071 41.7943 113.524 44.6459L118.925 41.8938C116.891 37.9017 113.645 34.656 109.653 32.6219L106.901 38.023ZM89.1095 36.3713C94.252 36.3713 97.9266 36.3736 100.807 36.609C103.652 36.8414 105.454 37.286 106.901 38.023L109.653 32.6219C107.209 31.3768 104.521 30.8303 101.301 30.5672C98.1161 30.307 94.152 30.3094 89.1095 30.3094V36.3713ZM56.3754 36.3713H89.1095V30.3094H56.3754V36.3713ZM38.5839 38.023C40.0304 37.286 41.8328 36.8414 44.6779 36.609C47.5583 36.3736 51.2329 36.3713 56.3754 36.3713V30.3094C51.3329 30.3094 47.3688 30.307 44.1842 30.5672C40.9643 30.8303 38.2754 31.3768 35.8318 32.6219L38.5839 38.023ZM31.961 44.6459C33.4139 41.7943 35.7323 39.476 38.5839 38.023L35.8318 32.6219C31.8397 34.656 28.5939 37.9017 26.5598 41.8939L31.961 44.6459ZM27.231 66.4469C25.5309 66.4469 24.1527 67.8251 24.1527 69.5252H30.2145C30.2145 71.1729 28.8787 72.5087 27.231 72.5087V66.4469ZM45.3414 103.94C45.9098 103.371 46.6807 103.052 47.4846 103.052V96.9901C45.073 96.9901 42.7602 97.9481 41.055 99.6533L45.3414 103.94ZM24.2474 69.4304C24.2474 67.7827 25.5832 66.4469 27.231 66.4469V72.5087C28.9311 72.5087 30.3093 71.1305 30.3093 69.4304H24.2474Z"
                  fill="#C7C7C7"
                />
                <path
                  d="M51.3477 57.3955L93.6393 57.3955"
                  stroke="#C7C7C7"
                  stroke-width="6.06188"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M51.3477 75.522L81.556 75.522"
                  stroke="#C7C7C7"
                  stroke-width="6.06188"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
              <span class="subtext d-block reviewers"
                >Your Reviews & Ratings are welcome!</span
              >
              <p class="cta">
                Share your thoughts on this property using the comment box
                above.
              </p>
            </div>
            <PropertyReviewList v-else style="margin-top: 60px" :edit="false" />
          </form>
        </div>
      </v-row>
    </v-container>
    <section id="similar-prop-view">
      <v-container data-aos="fade-up" data-aos-duration="500">
        <property-list
          title="Similar Listings"
          :properties="properties"
        ></property-list>
      </v-container>
    </section>
    <PropertyImageDialogue ref="imageModal" />
  </section>
</template>

<script>
export default {
  layout: "property",
  data() {
    return {
      showReview: false,
      contact: {
        name: "",
        email: "",
        phone: "",
        message: "",
      },
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
  methods: {
    showModal() {
      this.$refs.imageModal.showImgModal();
    },
  },
};
</script>

<style lang="scss" scoped>
#property-view {
  margin-top: -96px;
}

.property-view {
  margin-top: 117px;
}

.header_left {
  font-weight: 700;
  font-size: 2.4rem;
  color: var(--secondary-color);
}

.header_left p.header_subtext {
  font-weight: 500;
  font-size: 1.8rem;
  color: var(--property-subtext-color);
}

.propertyActionWrapper {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  gap: 17px;
}

.Btn {
  height: 4.8rem;
  border: 1px solid var(--border02-color);
  background: #fff !important;
  border-radius: 0 !important;
  box-shadow: none;
  text-transform: none;
}

.v-btn:not(.v-btn--round).v-size--default {
  height: 4.8rem;
}

.Btn svg {
  display: inline;
  margin-right: 8px;
}

.Btn span {
  font-weight: 500;
  color: var(--primary-color);
  font-size: 1.6rem;
}

.Btn:hover {
  border: 1px solid var(--primary-color);
  transition: all 0.2s linear;
}

.Btn:hover span {
  color: var(--secondary-color);
  transition: all 0.2s linear;
}

.Btn:hover svg path,
.Btn:hover svg circle {
  stroke: var(--secondary-color);
  transition: all 0.2s linear;
}

.Btn.viewMore {
  position: absolute;
  z-index: 3;
  bottom: 24px;
  text-transform: none;
  right: 16px;
  height: 4.8rem;
}

.Btn.reviewPost {
  background: var(--primary-color) !important;
  height: 4.2rem !important;
  min-width: 12.1rem !important;
  text-transform: none;
  margin-right: 24px !important;
}

.Btn.reviewPost.sm {
  margin-bottom: 30px;
  margin-right: 0;
  display: none;
}

.Btn.reviewPost:hover {
  border: none !important;
}

.Btn.reviewPost span {
  color: #fff;
}

.contact_wrapper a {
  text-decoration: none;
}

.contact_wrapper a .Btn.contact:hover svg path,
.contact_wrapper a .Btn.contact:hover svg circle {
  stroke: inherit;
  transition: all 0.2s linear;
}

.contact_wrapper .Btn.contact {
  height: 53px !important;
  width: 100% !important;
  justify-content: flex-start !important;
  text-transform: none;
}

.contact_wrapper a .Btn.contact.phone {
  background: var(--secondary-color) !important;
}

.contact_wrapper a .Btn.contact.phone:hover {
  border-color: var(--secondary-color) !important;
}

.contact_wrapper a .Btn.contact.whatsapp {
  border: 1px solid var(--contact02-color);
  background: rgba(37, 211, 102, 0.1) !important;
}

.contact_wrapper a .Btn.contact.phone span {
  color: #fff;
  font-weight: 700;
}

.contact_wrapper a .Btn.contact.whatsapp span {
  font-weight: 500;
  color: var(--contact02-color);
}

.PropImgWrapper {
  max-height: 48.1rem;
  cursor: pointer;
}
.PropImgWrapper.lg {
  padding-bottom: 0;
}
.PropImgWrapper iframe {
  width: 100%;
  height: 100%;
}

.PropImgWrapper.srow {
  padding: 12px 0 0 0;
}

.PropImgWrapper img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.smallPropImgWrapper {
  max-height: 22.5rem;
  // padding-bottom: 0;
  margin-bottom: 0;
  padding-right: 0;
}

.smallPropImgWrapper.box-2 {
  // margin-bottom: -18px;
}

.smallPropImgWrapper img {
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.features {
  min-height: 94px;
  height: 114px;
  border: 1px solid var(--border02-color);
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

.features aside {
  padding: 27px 0;
}

.features aside p {
  font-weight: 500;
  font-size: 1.6rem;
  color: var(--property-subtext-color);
}

.features aside > div span {
  font-weight: 700;
  font-size: 1.6rem;
  color: var(--property-span-color);
}

.features aside > div {
  display: flex;
  align-items: center;
  gap: 15px;
  height: 100%;
}

.contact_wrapper {
  padding: 12px 0 0 0;
  height: 114px;
}

.contactCol {
  padding: 0 0 7px 12px;
}

.about > div {
  padding-bottom: 51px;
  margin-bottom: 31px;
  border-bottom: 1px solid var(--border02-color);
}

.m3x0 header {
  font-weight: 700;
  font-size: 2.4rem;
  color: var(--secondary-color);
}

.m3x0 span.subtext {
  font-weight: 400;
  font-size: 1.8rem;
  color: var(--property-subtext-color);
}

.m3x0 span.propData {
  font-weight: 600;
  font-size: 1.8rem;
  color: var(--secondary-color);
}

.propInfo table {
  width: 100%;
}

.propInfo table tr td {
  padding-top: 20px;
}

.propInfo table tr:first-child td {
  padding-top: 0;
}

.amenties_wrapper {
  display: flex;
  align-items: center;
  gap: 10px;
  margin-bottom: 21px;
}

.amenties .amenties_wrapper:last-child {
  margin-bottom: 0;
}

.authCard {
  width: 100% !important;
  box-shadow: none !important;
  border: 1px solid var(--border02-color) !important;
  margin-left: 24px;
}

.modal_content .row_form input {
  height: 4.8rem;
}

.relative input {
  height: 5.8rem !important;
}

.placeholder {
  position: absolute;
  padding: 3px;
  color: rgba(57, 20, 0, 0.64);
  background-color: #fff;
  left: 22px;
  top: 26px;
  font-size: 15px;
  opacity: 1;
  text-transform: capitalize;
  cursor: auto;
}

input::placeholder,
textarea::placeholder {
  font-size: 12px;
  color: rgba(57, 20, 0, 0.64);
}

input + .placeholder {
  animation: unreveal-input 0.2s;
  animation-direction: reverse;
}

input:focus + .placeholder {
  top: 1px;
  left: 18px;
  font-size: 12px;
  color: var(--primary-color);
  animation: reveal-input 0.25s;
}

.containsElement.placeholder {
  top: 1px !important;
  left: 18px !important;
  font-size: 12px !important;
  color: var(--primary-color) !important;
}

@keyframes reveal-input {
  from {
    left: 22px;
    top: 22px;
    font-size: 15px;
  }

  to {
    top: 1px;
    left: 18px;
    font-size: 12px;
  }
}

@keyframes unreveal-input {
  from {
    left: 22px;
    top: 22px;
    font-size: 15px;
  }

  to {
    top: 1px;
    left: 18px;
    font-size: 12px;
  }
}

.footer {
  width: 100%;
}

.footer .Btn {
  width: 100%;
}

.locationSpace {
  height: 21.9rem;
  width: 100%;
  background: linear-gradient(
      93deg,
      rgba(191, 144, 1, 0.1) 0%,
      rgba(191, 144, 1, 0.1) 20%
    ),
    url(./images/pngs/mapStatic.png");
  background-size: cover;
  margin-top: 30px;
}

p.ratings {
  font-weight: 600;
  font-size: 2rem;
  color: var(--property-span-color);
}

.ratings_card {
  width: 100% !important;
  box-shadow: none !important;
  border: 1px solid var(--border02-color) !important;
  border-radius: 0 !important;
  display: flex !important;
  align-items: center;
  justify-content: center;
  height: 8.2rem;
  margin-bottom: 20px;
}

.ratings_card > div {
  display: flex;
  align-items: center;
  gap: 5px;
}

.ratings_card > div svg {
  cursor: pointer;
}

.no_reviews {
  text-align: center;
  margin-top: 60px;
  margin-bottom: 163px;
}

.no_reviews svg {
  display: inline;
}

p.cta {
  font-weight: 500;
  font-size: 1.6rem;
  color: var(--property-span-color);
}

div.col-12:has(.mobile) {
  display: none;
}

#similar-prop-view {
  background-color: var(--section-bg);
}

iframe {
  width: 100%;
}
</style>