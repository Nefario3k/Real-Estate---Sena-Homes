<template>
  <div id="contact-us">
    <section id="contactHeader">
      <aside class="contactHeader">
        <div>
          <header>Contact Us</header>
          <p>
            There are many variations of passages of Lorem Ipsum available but
            the this in majority have suffered alteration in some
          </p>
        </div>
      </aside>
    </section>
    <section id="get-in-touch">
      <aside class="mapFormSection relative">
        <v-container class="mapContainer">
          <v-row>
            <div class="col-12 col-md-5 col-md-5 col-xl-5">
              <v-card class="authCard" style="box-shadow: none">
                <div class="modal_content">
                  <form action="" class="content_area">
                    <header
                      class="text-left"
                      style="margin-bottom: 23px; color: var(--gei-color)"
                    >
                      Get In Touch
                    </header>
                    <v-row class="row_form">
                      <div class="relative col-12">
                        <input
                          id="fname"
                          required
                          autocomplete="off"
                          type="text"
                          name=""
                          v-model="contact.fullName"
                        />
                        <label
                          for="fname"
                          :class="{ containsElement: contact.fullName }"
                          class="placeholder"
                          >Full Name</label
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
                          >Your Email</label
                        >
                      </div>
                      <div class="relative col-12">
                        <input
                          id="subject"
                          required
                          autocomplete="off"
                          type="text"
                          name=""
                          v-model="contact.subject"
                        />
                        <label
                          for="subject"
                          :class="{ containsElement: contact.subject }"
                          class="placeholder"
                          >Subject</label
                        >
                      </div>
                      <div class="relative col-12">
                        <textarea
                          required
                          rows="5"
                          v-model="contact.message"
                          placeholder="Message"
                          cols=""
                        ></textarea>
                      </div>
                    </v-row>
                    <footer class="footer">
                      <v-btn class="Btn">Submit Now</v-btn>
                    </footer>
                  </form>
                </div>
              </v-card>
            </div>
            <div class="col-12 mapMobile d-none relative">
              <a
                href="https://www.google.com/maps/place/Al+Shoala+Building+-+Port+Saeed+-+Dubai+-+United+Arab+Emirates/@25.2545311,55.3293408,17z/data=!4m6!3m5!1s0x3e5f5cd8e7197c75:0x9c7e62633c2ce47c!8m2!3d25.2545311!4d55.3293408!16s%2Fg%2F11b6bpyh5n"
                target="_blank"
                class="mapIcon"
              >
                <svg
                  width="72"
                  height="90"
                  viewBox="0 0 72 90"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M72 36C72 55.8823 55.5 80 36 89.5C17.5 81.5 0 55.8823 0 36C0 16.1177 16.1177 0 36 0C55.8823 0 72 16.1177 72 36Z"
                    fill="#1C212B"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M48 41C48 49.628 36 61 36 61C36 61 24 49.628 24 41C24 34.3726 29.3726 29 36 29C42.6274 29 48 34.3726 48 41ZM30 41C30 44.3137 32.6863 47 36 47C39.3137 47 42 44.3137 42 41C42 37.6863 39.3137 35 36 35C32.6863 35 30 37.6863 30 41Z"
                    fill="white"
                  />
                </svg>
              </a>
            </div>
          </v-row>
          <a
            href="https://www.google.com/maps/place/Al+Shoala+Building+-+Port+Saeed+-+Dubai+-+United+Arab+Emirates/@25.2545311,55.3293408,17z/data=!4m6!3m5!1s0x3e5f5cd8e7197c75:0x9c7e62633c2ce47c!8m2!3d25.2545311!4d55.3293408!16s%2Fg%2F11b6bpyh5n"
            target="_blank"
            class="mapIcon"
          >
            <svg
              width="72"
              height="90"
              viewBox="0 0 72 90"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M72 36C72 55.8823 55.5 80 36 89.5C17.5 81.5 0 55.8823 0 36C0 16.1177 16.1177 0 36 0C55.8823 0 72 16.1177 72 36Z"
                fill="#1C212B"
              />
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M48 41C48 49.628 36 61 36 61C36 61 24 49.628 24 41C24 34.3726 29.3726 29 36 29C42.6274 29 48 34.3726 48 41ZM30 41C30 44.3137 32.6863 47 36 47C39.3137 47 42 44.3137 42 41C42 37.6863 39.3137 35 36 35C32.6863 35 30 37.6863 30 41Z"
                fill="white"
              />
            </svg>
          </a>
        </v-container>
      </aside>
      <v-container class="contactInfoContainer">
        <v-row class="contact_row">
          <div class="col-12 col-md-4 col-lg-4 col-xl-4">
            <div class="contact_info">
              <div class="contact_title">
                <svg
                  width="63"
                  height="64"
                  viewBox="0 0 63 64"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <ellipse
                    cx="31.5157"
                    cy="32"
                    rx="30.6063"
                    ry="32"
                    fill="#BF9001"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M22.7435 20.7653C23.2513 20.2352 23.9522 19.9583 24.6684 20.0051C25.3846 20.0519 26.0471 20.4177 26.4879 21.0098L29.063 24.469C29.535 25.1035 29.7015 25.93 29.515 26.7101L28.7302 29.9952C28.6477 30.3413 28.7446 30.7073 28.9856 30.9598L32.5105 34.6454C32.7522 34.8979 33.1029 34.9993 33.4344 34.9124L36.5748 34.0919C37.3207 33.8969 38.111 34.0711 38.7181 34.5644L42.0263 37.2555C43.2156 38.2231 43.3247 40.0607 42.2602 41.1722L40.7768 42.7233C39.7152 43.8333 38.1285 44.3209 36.6494 43.7763C32.8636 42.3836 29.4264 40.1174 26.5926 37.146C23.751 34.1834 21.5838 30.5899 20.2516 26.6321C19.7322 25.087 20.1985 23.4264 21.2601 22.3164L22.7435 20.7653Z"
                    fill="white"
                  />
                </svg>
                <p>phone</p>
              </div>
              <p class="contact_information">
                <a href="tel:+971586276573">+(971) 586-276-573</a>
              </p>
            </div>
          </div>
          <div class="col-12 col-md-4 col-lg-4 col-xl-4">
            <div class="contact_info middlem">
              <div class="contact_title">
                <svg
                  width="63"
                  height="64"
                  viewBox="0 0 63 64"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <ellipse
                    cx="31.5301"
                    cy="32"
                    rx="30.6063"
                    ry="32"
                    fill="#BF9001"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M22.922 23C21.5832 22.9999 20.4223 23.9678 20.1244 25.3325L31.5301 32.621L42.9357 25.3325C42.6378 23.9678 41.4769 22.9999 40.1381 23H22.922ZM20.053 37.7015V27.0455L28.3784 32.3645L20.053 37.7015ZM29.7525 33.245L20.3267 39.2855C20.8021 40.3335 21.8127 41.0011 22.9221 41H40.1381C41.2473 41.0002 42.2573 40.3321 42.732 39.284L33.3062 33.2435L31.5301 34.379L29.7525 33.2435V33.245ZM43.0074 37.7015L34.682 32.366V32.3645L43.0074 27.0455V37.7015Z"
                    fill="white"
                  />
                </svg>
                <p>Email</p>
              </div>
              <p class="contact_information">
                <a href="mailto:info@senahomesrealestate.com"
                  >info@senahomesrealestate.com</a
                >
              </p>
            </div>
          </div>
          <div class="col-12 col-md-4 col-lg-4 col-xl-4">
            <div class="contact_info">
              <div class="contact_title">
                <svg
                  width="63"
                  height="64"
                  viewBox="0 0 63 64"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <ellipse
                    cx="31.5448"
                    cy="32"
                    rx="30.6063"
                    ry="32"
                    fill="#BF9001"
                  />
                  <g clip-path="url(#clip0_0_1)">
                    <path
                      d="M40.1004 21.1512L22.2349 29.3969C20.1737 30.359 20.8607 33.3822 23.0595 33.3822H30.6181V40.9409C30.6181 43.1396 33.6414 43.8271 34.6034 41.7654L42.8491 23.8999C43.5362 22.2503 41.7496 20.4637 40.1004 21.1512Z"
                      fill="white"
                    />
                  </g>
                  <defs>
                    <clipPath id="clip0_0_1">
                      <rect
                        width="22"
                        height="22"
                        fill="white"
                        transform="translate(21 21)"
                      />
                    </clipPath>
                  </defs>
                </svg>
                <p>address</p>
              </div>
              <p class="contact_information">
                <a href="https://goo.gl/maps/R4WHukmvi36pREhp6" target="_blank"
                  >Al shoala Building, Port Saeed, Dubai, UAE</a
                >
              </p>
            </div>
          </div>
          <div style="overflow: hidden" class="col-12 geiSocials">
            <div data-aos="fade-left" data-aos-duration="500" class="socialIco">
              <nuxt-link to="" title="Facebook">
                <svg
                  width="42"
                  height="42"
                  viewBox="0 0 42 42"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="21" cy="21" r="21" fill="#BF9001" />
                  <path
                    d="M24.51 14.32H26.39V11.14C25.4798 11.0454 24.5652 10.9986 23.65 11C20.93 11 19.07 12.66 19.07 15.7V18.32H16V21.88H19.07V31H22.75V21.88H25.81L26.27 18.32H22.75V16.05C22.75 15 23.03 14.32 24.51 14.32Z"
                    fill="white"
                  />
                </svg>
              </nuxt-link>
            </div>
            <div data-aos="fade-left" data-aos-duration="900" class="socialIco">
              <nuxt-link to="" title="Instagram">
                <svg
                  width="42"
                  height="42"
                  viewBox="0 0 42 42"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="21" cy="21" r="21" fill="#BF9001" />
                  <path
                    d="M26.34 14.46C26.1027 14.46 25.8707 14.5304 25.6733 14.6622C25.476 14.7941 25.3222 14.9815 25.2313 15.2008C25.1405 15.4201 25.1168 15.6613 25.1631 15.8941C25.2094 16.1269 25.3236 16.3407 25.4915 16.5085C25.6593 16.6764 25.8731 16.7906 26.1059 16.8369C26.3387 16.8832 26.5799 16.8595 26.7992 16.7687C27.0185 16.6778 27.2059 16.524 27.3378 16.3267C27.4696 16.1293 27.54 15.8973 27.54 15.66C27.54 15.3417 27.4136 15.0365 27.1885 14.8115C26.9635 14.5864 26.6583 14.46 26.34 14.46ZM30.94 16.88C30.9206 16.0503 30.7652 15.2294 30.48 14.45C30.2257 13.7831 29.83 13.1793 29.32 12.68C28.8248 12.1674 28.2196 11.7742 27.55 11.53C26.7727 11.2362 25.9508 11.0772 25.12 11.06C24.06 11 23.72 11 21 11C18.28 11 17.94 11 16.88 11.06C16.0492 11.0772 15.2273 11.2362 14.45 11.53C13.7817 11.7766 13.1769 12.1696 12.68 12.68C12.1674 13.1752 11.7742 13.7804 11.53 14.45C11.2362 15.2273 11.0772 16.0492 11.06 16.88C11 17.94 11 18.28 11 21C11 23.72 11 24.06 11.06 25.12C11.0772 25.9508 11.2362 26.7727 11.53 27.55C11.7742 28.2196 12.1674 28.8248 12.68 29.32C13.1769 29.8304 13.7817 30.2234 14.45 30.47C15.2273 30.7638 16.0492 30.9228 16.88 30.94C17.94 31 18.28 31 21 31C23.72 31 24.06 31 25.12 30.94C25.9508 30.9228 26.7727 30.7638 27.55 30.47C28.2196 30.2258 28.8248 29.8326 29.32 29.32C29.8322 28.8226 30.2283 28.2182 30.48 27.55C30.7652 26.7706 30.9206 25.9497 30.94 25.12C30.94 24.06 31 23.72 31 21C31 18.28 31 17.94 30.94 16.88ZM29.14 25C29.1327 25.6348 29.0178 26.2637 28.8 26.86C28.6403 27.2952 28.3839 27.6884 28.05 28.01C27.7256 28.3405 27.3332 28.5964 26.9 28.76C26.3037 28.9778 25.6748 29.0927 25.04 29.1C24.04 29.15 23.67 29.16 21.04 29.16C18.41 29.16 18.04 29.16 17.04 29.1C16.3809 29.1123 15.7246 29.0109 15.1 28.8C14.6858 28.6281 14.3114 28.3728 14 28.05C13.6681 27.7287 13.4148 27.3352 13.26 26.9C13.0159 26.2952 12.8804 25.6519 12.86 25C12.86 24 12.8 23.63 12.8 21C12.8 18.37 12.8 18 12.86 17C12.8645 16.3511 12.983 15.7079 13.21 15.1C13.386 14.6779 13.6563 14.3017 14 14C14.3038 13.6562 14.6793 13.3831 15.1 13.2C15.7096 12.98 16.352 12.8651 17 12.86C18 12.86 18.37 12.8 21 12.8C23.63 12.8 24 12.8 25 12.86C25.6348 12.8673 26.2637 12.9822 26.86 13.2C27.3144 13.3687 27.7223 13.6428 28.05 14C28.3777 14.3072 28.6338 14.6827 28.8 15.1C29.0223 15.7089 29.1373 16.3518 29.14 17C29.19 18 29.2 18.37 29.2 21C29.2 23.63 29.19 24 29.14 25ZM21 15.87C19.9858 15.872 18.995 16.1745 18.1527 16.7394C17.3103 17.3043 16.6544 18.1062 16.2676 19.0438C15.8809 19.9813 15.7807 21.0125 15.9798 22.0069C16.1789 23.0014 16.6682 23.9145 17.3861 24.631C18.1039 25.3474 19.018 25.835 20.0129 26.0321C21.0077 26.2293 22.0387 26.1271 22.9755 25.7385C23.9123 25.35 24.7129 24.6924 25.2761 23.849C25.8394 23.0056 26.14 22.0142 26.14 21C26.1413 20.3251 26.0092 19.6566 25.7512 19.033C25.4933 18.4093 25.1146 17.8428 24.6369 17.3661C24.1592 16.8893 23.5919 16.5117 22.9678 16.2549C22.3436 15.9982 21.6749 15.8674 21 15.87ZM21 24.33C20.3414 24.33 19.6976 24.1347 19.15 23.7688C18.6023 23.4029 18.1755 22.8828 17.9235 22.2743C17.6714 21.6659 17.6055 20.9963 17.734 20.3503C17.8625 19.7044 18.1796 19.111 18.6453 18.6453C19.111 18.1796 19.7044 17.8625 20.3503 17.734C20.9963 17.6055 21.6659 17.6714 22.2743 17.9235C22.8828 18.1755 23.4029 18.6023 23.7688 19.15C24.1347 19.6976 24.33 20.3414 24.33 21C24.33 21.4373 24.2439 21.8703 24.0765 22.2743C23.9092 22.6784 23.6639 23.0454 23.3547 23.3547C23.0454 23.6639 22.6784 23.9092 22.2743 24.0765C21.8703 24.2439 21.4373 24.33 21 24.33Z"
                    fill="white"
                  />
                </svg>
              </nuxt-link>
            </div>
            <div
              data-aos="fade-left"
              data-aos-duration="1300"
              class="socialIco"
            >
              <nuxt-link to="" title="Twitter">
                <svg
                  width="42"
                  height="42"
                  viewBox="0 0 42 42"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="21" cy="21" r="21" fill="#BF9001" />
                  <path
                    d="M31 14.8002C30.2483 15.1263 29.4534 15.3419 28.64 15.4402C29.4982 14.9275 30.1413 14.121 30.45 13.1702C29.6436 13.6503 28.7608 13.9885 27.84 14.1702C27.2245 13.5028 26.405 13.0585 25.5098 12.9071C24.6147 12.7556 23.6945 12.9056 22.8938 13.3334C22.093 13.7612 21.4569 14.4427 21.0852 15.271C20.7135 16.0994 20.6273 17.0276 20.84 17.9102C19.2094 17.8277 17.6144 17.4032 16.1587 16.6641C14.7029 15.925 13.4188 14.8879 12.39 13.6202C12.0291 14.2504 11.8395 14.964 11.84 15.6902C11.8387 16.3646 12.0042 17.0288 12.3218 17.6238C12.6393 18.2187 13.099 18.7259 13.66 19.1002C13.008 19.0825 12.3699 18.9075 11.8 18.5902V18.6402C11.8049 19.5851 12.136 20.4993 12.7373 21.2282C13.3386 21.957 14.1733 22.4559 15.1 22.6402C14.7433 22.7488 14.3729 22.806 14 22.8102C13.7419 22.8072 13.4844 22.7838 13.23 22.7402C13.4939 23.553 14.0046 24.2634 14.6911 24.7724C15.3775 25.2814 16.2056 25.5638 17.06 25.5802C15.6172 26.7155 13.8359 27.3351 12 27.3402C11.6657 27.3413 11.3317 27.3213 11 27.2802C12.8744 28.4905 15.0588 29.1329 17.29 29.1302C18.8297 29.1462 20.3571 28.8552 21.7831 28.2743C23.2091 27.6934 24.505 26.8341 25.5952 25.7467C26.6854 24.6593 27.548 23.3656 28.1326 21.9411C28.7172 20.5166 29.012 18.9899 29 17.4502C29 17.2802 29 17.1002 29 16.9202C29.7847 16.335 30.4615 15.6176 31 14.8002Z"
                    fill="white"
                  />
                </svg>
              </nuxt-link>
            </div>
            <div
              data-aos="fade-left"
              data-aos-duration="1700"
              class="socialIco"
            >
              <nuxt-link to="" title="Linkeldn">
                <svg
                  width="42"
                  height="42"
                  viewBox="0 0 42 42"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="21" cy="21" r="21" fill="#BF9001" />
                  <path
                    d="M29.4701 11.0001H12.5301C12.3396 10.9975 12.1506 11.0324 11.9736 11.1028C11.7967 11.1733 11.6354 11.2779 11.4989 11.4107C11.3624 11.5434 11.2533 11.7018 11.1781 11.8767C11.1028 12.0517 11.0627 12.2397 11.0601 12.4301V29.5701C11.0627 29.7606 11.1028 29.9486 11.1781 30.1235C11.2533 30.2985 11.3624 30.4568 11.4989 30.5896C11.6354 30.7224 11.7967 30.827 11.9736 30.8975C12.1506 30.9679 12.3396 31.0028 12.5301 31.0001H29.4701C29.6605 31.0028 29.8496 30.9679 30.0265 30.8975C30.2034 30.827 30.3648 30.7224 30.5013 30.5896C30.6378 30.4568 30.7468 30.2985 30.8221 30.1235C30.8974 29.9486 30.9375 29.7606 30.9401 29.5701V12.4301C30.9375 12.2397 30.8974 12.0517 30.8221 11.8767C30.7468 11.7018 30.6378 11.5434 30.5013 11.4107C30.3648 11.2779 30.2034 11.1733 30.0265 11.1028C29.8496 11.0324 29.6605 10.9975 29.4701 11.0001ZM17.0901 27.7401H14.0901V18.7401H17.0901V27.7401ZM15.5901 17.4801C15.1763 17.4801 14.7795 17.3158 14.487 17.0232C14.1944 16.7307 14.0301 16.3339 14.0301 15.9201C14.0301 15.5064 14.1944 15.1096 14.487 14.8171C14.7795 14.5245 15.1763 14.3601 15.5901 14.3601C15.8098 14.3352 16.0322 14.357 16.2429 14.424C16.4536 14.4911 16.6478 14.6018 16.8127 14.7491C16.9776 14.8964 17.1096 15.0768 17.1999 15.2786C17.2903 15.4804 17.337 15.699 17.337 15.9201C17.337 16.1412 17.2903 16.3599 17.1999 16.5617C17.1096 16.7635 16.9776 16.9439 16.8127 17.0912C16.6478 17.2385 16.4536 17.3492 16.2429 17.4163C16.0322 17.4833 15.8098 17.5051 15.5901 17.4801ZM27.9101 27.7401H24.9101V22.9101C24.9101 21.7001 24.4801 20.9101 23.3901 20.9101C23.0527 20.9126 22.7242 21.0184 22.4489 21.2133C22.1735 21.4082 21.9645 21.6828 21.8501 22.0001C21.7718 22.2352 21.7379 22.4827 21.7501 22.7301V27.7301H18.7501C18.7501 27.7301 18.7501 19.5501 18.7501 18.7301H21.7501V20.0001C22.0226 19.5272 22.419 19.1377 22.8965 18.8733C23.374 18.609 23.9146 18.48 24.4601 18.5001C26.4601 18.5001 27.9101 19.7901 27.9101 22.5601V27.7401Z"
                    fill="white"
                  />
                </svg>
              </nuxt-link>
            </div>
            <div
              data-aos="fade-left"
              data-aos-duration="2100"
              class="socialIco"
            >
              <nuxt-link to="" title="Whatsapp">
                <svg
                  width="42"
                  height="42"
                  viewBox="0 0 42 42"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <circle cx="21" cy="21" r="21" fill="#BF9001" />
                  <g clip-path="url(#clip0_1_15915)">
                    <path
                      d="M28.4486 13.2618C26.391 11.1993 23.6508 10.0649 20.7387 10.0649C14.728 10.0649 9.83696 14.956 9.83696 20.9667C9.83696 22.8868 10.3378 24.7627 11.2905 26.4176L9.74365 32.0649L15.5236 30.5475C17.1146 31.4167 18.907 31.8734 20.7338 31.8734H20.7387C26.7445 31.8734 31.7437 26.9824 31.7437 20.9716C31.7437 18.0596 30.5062 15.3243 28.4486 13.2618ZM20.7387 30.0368C19.1084 30.0368 17.5124 29.5998 16.1227 28.7748L15.7937 28.5783L12.366 29.477L13.2794 26.1328L13.0633 25.789C12.1548 24.3453 11.6785 22.6806 11.6785 20.9667C11.6785 15.9725 15.7445 11.9065 20.7437 11.9065C23.1646 11.9065 25.4383 12.8493 27.1472 14.5632C28.8562 16.277 29.907 18.5507 29.9021 20.9716C29.9021 25.9707 25.7329 30.0368 20.7387 30.0368ZM25.7084 23.2502C25.4383 23.1127 24.0977 22.4547 23.8472 22.3663C23.5968 22.273 23.4151 22.2288 23.2334 22.5038C23.0517 22.7788 22.5312 23.3877 22.3691 23.5743C22.212 23.756 22.0499 23.7806 21.7798 23.6431C20.1789 22.8426 19.128 22.214 18.0722 20.402C17.7923 19.9207 18.3521 19.9551 18.8727 18.914C18.9611 18.7324 18.9169 18.5752 18.8481 18.4377C18.7794 18.3002 18.2343 16.9596 18.0084 16.4145C17.7874 15.8841 17.5615 15.9578 17.3945 15.948C17.2374 15.9382 17.0557 15.9382 16.874 15.9382C16.6923 15.9382 16.3977 16.0069 16.1472 16.277C15.8968 16.552 15.1945 17.21 15.1945 18.5507C15.1945 19.8913 16.1718 21.1877 16.3044 21.3694C16.4419 21.5511 18.2245 24.3011 20.9597 25.4846C22.6883 26.231 23.366 26.2949 24.2303 26.1672C24.7557 26.0886 25.841 25.5091 26.0669 24.8707C26.2928 24.2324 26.2928 23.6873 26.224 23.5743C26.1602 23.4515 25.9785 23.3828 25.7084 23.2502Z"
                      fill="white"
                    />
                  </g>
                  <defs>
                    <clipPath id="clip0_1_15915">
                      <rect
                        width="22"
                        height="22"
                        fill="white"
                        transform="translate(10 10)"
                      />
                    </clipPath>
                  </defs>
                </svg>
              </nuxt-link>
            </div>
          </div>
        </v-row>
      </v-container>
    </section>
    <FAQ />
    <FindBestRE />
    <MobileApp />
  </div>
</template>

<script>
export default {
  data() {
    return {
      contact: {
        fullName: "",
        email: "",
        subject: "",
        message: "",
      },
    };
  },
};
</script>

<style scoped>
/* pages animation  */
#contact-us {
  animation: transIn 0.8s linear 0s;
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
#contactHeader {
  background: linear-gradient(
      93deg,
      rgba(28, 33, 43, 0.7) 0%,
      rgba(28, 33, 43, 0.7) 20%
    ),
    url(./images/pngs/contactHeader.png");
  background-size: cover;
  width: 100%;
  min-height: 40rem;
  margin-top: -96px;
}
.contactHeader {
  min-height: 40rem;
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.contactHeader header {
  color: #fff;
  font-size: 5.4rem;
  font-weight: 700;
  margin-top: 90px;
  margin-bottom: 24px;
}
.contactHeader p {
  font-weight: 400;
  font-size: 1.8rem;
  color: #fff;
  width: 60%;
  margin: 0 auto;
  mix-blend-mode: normal;
  opacity: 0.7;
}
.mapFormSection {
  min-height: 72.4rem;
  background: linear-gradient(
      93deg,
      rgba(191, 144, 1, 0.1) 0%,
      rgba(191, 144, 1, 0.1) 20%
    ),
    url(./images/pngs/mapStatic.png");
  background-size: cover;
  background-repeat: no-repeat;
  /* overflow: hidden; */
}
.mapIcon {
  position: absolute;
  right: 32%;
  top: 50%;
  transform: translateY(-50%);
}
.mapContainer {
  display: flex;
  padding-top: 81px;
  padding-bottom: 82px;
  align-items: center;
}
.modal_content .row_form {
  margin-bottom: 25px;
}
.modal_content .row_form input {
  height: 4.8rem;
}
.placeholder {
  position: absolute;
  padding: 3px;
  color: rgba(57, 20, 0, 0.64);
  background-color: #fff;
  left: 22px;
  top: 22px;
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
  width: 15.4rem;
}
.contactInfoContainer {
  display: flex;
  align-items: center;
  margin-top: 80px;
  margin-bottom: 72px;
}
.contact_row:has(.col-12) {
  width: 80% !important;
  margin-left: auto;
  margin-right: auto;
}
.contact_info {
  min-height: 19.2rem;
  padding: 32px 12px 32px 46px;
}
.col-12:has(.contact_info) {
  border: 1px solid var(--contact-color);
}
.contact_title {
  display: flex;
  align-items: center;
  gap: 23px;
  margin-bottom: 26px;
}
.contact_title p {
  font-weight: 400;
  font-size: 1.6rem;
  text-transform: uppercase;
  color: var(--primary-color);
  margin: 0;
}
.contact_information a {
  color: var(--gei-color);
  font-weight: 400;
  font-size: 1.8rem;
  word-wrap: break-word;
  text-decoration: none;
}
.contact_information a:hover {
  color: var(--primary-color);
}
.geiSocials {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
  margin-top: 50px;
}
.geiSocials a:hover svg circle {
  fill: var(--label-color);
  transition: all 0.2s linear;
}
.col-12:has(.middlem) {
  border-left: none;
  border-right: none;
}
@media (max-width: 959px) {
  .col-12:has(.middlem) {
    border: 1px solid var(--contact-color);
    border-top: none;
    border-bottom: none;
  }
  .contact_info {
    padding: 32px 12px 32px 28px;
  }
  .mapFormSection {
    background: #fff;
  }
  .mapContainer {
    padding-bottom: 12px;
  }
  .authCard {
    border: 1px solid var(--contact-color);
  }
  .mapMobile {
    display: block !important;
    height: 48.1rem;
    padding-left: 0;
    padding-right: 0;
    background: linear-gradient(
        93deg,
        rgba(191, 144, 1, 0.1) 0%,
        rgba(191, 144, 1, 0.1) 20%
      ),
      url(./images/pngs/mapStatic.png");
    background-size: cover;
    background-repeat: no-repeat;
  }

  .mapIcon {
    display: none;
  }
  .mapMobile .mapIcon {
    display: block;
  }
  .contact_information a {
    font-size: 1.6rem;
  }
  .geiSocials .socialIco svg {
    width: 30px;
    height: 30px;
  }
}
</style>