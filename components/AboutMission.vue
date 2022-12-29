<template>
  <div>
    <v-container>
      <div class="vision-mission">
        <div data-aos="fade-right" data-aos-duration="800" class="mission">
          <h3 data-aos="fade-up" data-aos-duration="1400">Our Mission</h3>
          <p data-aos="fade-up" data-aos-duration="1400">
            To offer quality driven, excellent and, superior customer experience
            by combining entrepreneurial aptitude, innovative strategies and
            bespoke service to guarantee client satisfaction that results in
            long lasting partnership. We pride ourselves on flawless integrity
            and loyalty to our clients.
          </p>
        </div>
        <div
          data-aos="fade-left"
          data-aos-duration="800"
          class="vision"
          style="box-shadow: 0px 6.33185px 12.6637px rgba(191, 144, 1, 0.09)"
        >
          <h3
            data-aos="fade-up"
            data-aos-duration="1400"
            style="color: var(--primary-color)"
          >
            Our Vision
          </h3>
          <p data-aos="fade-up" data-aos-duration="1400" style="color: #333333">
            To be the topmost leading service provider in the real estate
            industry and to make Sena Homes the first choice of every property
            seeker. We are committed to meeting the needs of our clients.
          </p>
        </div>
      </div>
    </v-container>
  </div>
</template>
<script>
// import bgImage from 'images/pngs/villa1.jpg';
export default {};
</script>
<style lang="scss" scoped>
.vision-mission {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-top: 10.9rem;
  padding-bottom: 12.1rem;
  overflow: hidden;

  div {
    max-width: 544px;
    padding: 4rem;
    font-size: 1.8rem;
    text-align: center;
    line-height: 3rem;
    font-weight: 300;
    border: 1px solid #d3dee8;
    box-sizing: border-box;

    h3 {
      margin: 2rem 0rem 4rem 0rem;
    }

    &.mission {
      background-color: #bf9001;
      color: white;
      margin-bottom: 4rem;
    }
  }
}

// => 'sm': '640px',
@media (min-width: 640px) {
}

// => 'md': '768px',
@media (min-width: 768px) {
  .vision-mission {
    flex-direction: row;
    column-gap: 3rem;
    margin-top: 10.9rem;
    padding-bottom: 12.1rem;

    div {
      max-width: 544px;
      padding: 4rem;
      font-size: 1.8rem;
      text-align: center;
      line-height: 3rem;
      font-weight: 300;
      border: 1px solid #d3dee8;
      box-sizing: border-box;
      min-height: 37rem;

      h3 {
        margin: 2rem 0rem 4rem 0rem;
      }

      &.mission {
        background-color: #bf9001;
        color: white;
        margin-bottom: 0rem;
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
@media (max-width: 540px) {
  .vision-mission {
    .mission {
      padding: 12px !important;
      padding-bottom: 26px !important;
      h3 {
        margin-bottom: 24px !important;
        font-size: 1.6rem !important;
      }
      p {
        font-size: 1.4rem !important;
        line-height: 19px !important;
        width: 90%;
        margin: auto;
      }
    }
  }
  .vision {
    padding: 12px !important;
    padding-bottom: 74px !important;
    h3 {
      margin-bottom: 32px !important;
      font-size: 1.6rem !important;
    }
    p {
      font-size: 1.4rem !important;
      line-height: 19px !important;
      width: 87%;
      margin: auto;
    }
  }
}
</style>