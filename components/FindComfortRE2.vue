<template>
  <div class="MSection">
    <img src="/images/svg/spiral.svg" class="bgImg" alt="" />
    <v-container class="section">
      <v-row class="comfortRow">
        <div class="col-12 right md d-none text-center">
          <p class="titleText">WHO WE ARE.</p>
          <h3>Sena Homes Real Estate</h3>
        </div>
        <div class="col-12 col-lg-6 col-xl-6 left">
          <div class="img-frame">
            <div class="tilted-box">
              <img src="/images/pngs/aboutWe.png" class="img" alt="" />
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-6 col-xl-6 right dd">
          <p class="titleText">WHO WE ARE.</p>
          <h3>Sena Homes Real Estate</h3>
          <div class="longTalk">
            <p>
              SENA Homes Real Estate is a property consultancy firm based in
              Dubai tailored to serve the challenging demands in the realty
              industry. We deal in Residential and commercial properties and aim
              to provide the best properties that work within the client’s
              criteria. Our team members are expert realtors who go the extra
              mile to provide best property options to the clients.
              <br />
              <br />
              SENA Homes Real Estate is a RERA-licensed Organization established
              by professionalism, integrity, accountability, and quality service
              giving you the most profitable Quick Sale/rental Solutions today.
              We have a vision of providing our clients with an unparalleled
              experience.
            </p>
          </div>
          <div class="btnWrapper">
            <v-btn class="custom-btn">Give Us a Call</v-btn>
          </div>
        </div>
      </v-row>
      <div class="right"></div>
    </v-container>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.MSection {
  position: relative;
  // background-image: url("/images/svg/spiral.svg");
  // background-position: top -10% right;
  background-color: #fff;
  overflow-y: hidden;
  .bgImg {
    position: absolute;
    filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
    opacity: 0.15;
    top: -10%;
    right: 0;
  }
}
.section {
  min-height: 80rem;
  // display: flex;
  // justify-content: center;
  padding-top: 91px;
  .left {
    position: relative;

    .img-frame {
      top: 0;
      left: 0;
      position: relative;
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;

      .tilted-box {
        position: relative;
        z-index: 1;
        width: 47rem;
        height: 70rem;
        left: 5rem;
        border: 9px solid rgba(191, 144, 1, 0.3);
        transform: rotate(-3deg);
      }

      .img {
        position: relative;
        z-index: 2;
        left: -2rem;
        top: -1rem;
        height: 100%;
        transform: rotate(3deg);
        // filter: drop-shadow(0px 44.6111px 133.833px rgba(50, 8, 8, 0.06));
      }
    }
  }

  .right {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;

    > img {
      position: absolute;
      right: 0;
      bottom: 0;
    }
    .titleText {
      color: var(--primary-color);
      font-weight: 400;
      font-size: 1.8rem;
    }

    h3 {
      font-weight: 700;
      font-size: 40px;
      line-height: 54px;
      color: #1c212b;
      margin-bottom: 40px;
    }
    .longTalk {
      width: 95%;
      p {
        margin: 0;
        font-weight: 400;
        font-size: 1.8rem;
        color: var(--secondary-color);
      }
    }
    .custom-btn {
      width: 21.3rem;
      height: 5.1rem;
      background: var(--primary-color);
      font-weight: 700;
      font-size: 16px;
      line-height: 36px;
      color: #ffffff;
      margin-top: 5rem;
      text-transform: capitalize;
      border-radius: 0;
      box-shadow: none;
    }
  }
}
@media (max-width: 1263px) {
  .section {
    padding-top: 59px;
    padding-bottom: 68px;
  }
  .left {
    min-height: 75rem !important;
    .tilted-box {
      left: 0 !important;
    }
    .img {
      left: 0 !important;
    }
  }
  .right.md {
    display: block !important;
  }
  .right.dd {
    text-align: center;
    h3,
    .titleText {
      display: none !important;
    }
    .longTalk {
      margin: auto;
    }
    .btnWrapper {
      text-align: center;
      .custom-btn {
        margin-top: 3rem !important;
        width: 22.7rem !important;
      }
    }
  }
}
@media (max-width: 959px) {
  .comfortRow {
    margin: 0 !important;
  }
}
@media (max-width: 560px) {
  .img-frame {
    margin-bottom: 30px;
  }
  .left {
    min-height: 40rem !important;
    .tilted-box {
      width: 90% !important;
      left: 1rem !important;
    }
    .img {
      height: 102% !important;
      width: 103% !important;
      object-fit: cover;
      left: -3rem !important;
    }
  }
  .right {
    h3 {
      font-size: 2.4rem !important;
    }
    .titleText {
      font-size: 1.6rem !important;
    }
  }
}
@media (max-width: 390px) {
  .left {
    min-height: 40rem !important;
    .tilted-box {
      height: 44.7rem !important;
    }
    .img {
      height: 102% !important;
      width: 103% !important;
      object-fit: cover;
      left: -3rem !important;
    }
  }
}
</style>
