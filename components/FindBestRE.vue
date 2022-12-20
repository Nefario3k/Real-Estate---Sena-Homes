<template>
  <div class="section">
    <h3 data-aos="fade-up" data-aos-duration="500" style="margin-bottom: 0">
      Find your best
    </h3>
    <h3 data-aos="fade-up" data-aos-duration="1000">Real Estate</h3>
    <p>
      We provide a complete service for the sale, <br />Purchase or rental of
      real estate.
    </p>
    <v-btn class="custom-btn">Browse Properties</v-btn>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.section {
  width: 100%;
  height: 65rem;
  box-sizing: border-box;
  background: linear-gradient(
      93deg,
      rgba(28, 33, 43, 0.7) 0%,
      rgba(28, 33, 43, 0.7) 20%
    ),
    url(./images/pngs/CTA.png") no-repeat;
  background-size: cover;
  background-color: var(--secondary-color);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: #ffffff;

  h3 {
    font-weight: 700;
    font-size: 54px;
    line-height: 55px;
    margin-bottom: 33px;
  }

  p {
    font-weight: 400;
    font-size: 22px;
    line-height: 36px;
    margin-bottom: 33px;
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
}

@media (max-width: 959px) {
  .section {
    width: 100%;
    height: 40rem;
    background: url(./images/pngs/burj-khalifa.png") no-repeat;
    background-size: cover;
    background-position: bottom;

    h3 {
      font-size: 32px;
      line-height: 33px;
    }

    p {
      font-size: 16px;
      line-height: 28px;
    }

    .custom-btn {
      width: 227px;
      font-size: 16px;
      font-weight: 500;
    }
  }
}
</style>
