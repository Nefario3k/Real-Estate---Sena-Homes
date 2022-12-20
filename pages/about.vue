<template>
  <div id="about">
    <section id="aboutHeader">
      <aside class="aboutHeader">
        <div>
          <header>About</header>
          <p>
            There are many variations of passages of Lorem Ipsum available but
            the this in majority have suffered alteration in some
          </p>
        </div>
      </aside>
    </section>
    <FindComfortRE2 />
    <section>
      <about-mission />
    </section>
    <section id="choice">
      <v-container>
        <div class="contentChoice">
          <p data-aos="fade-right" data-aos-duration="400" class="goldText">
            WHY CHOOSE US.
          </p>
          <header data-aos="fade-up" data-aos-duration="400">
            Why Sena Homes Real Estate?
          </header>
          <p data-aos="fade-up" data-aos-duration="800" class="content">
            With a desire for superiority in all our ventures, SENA HOMES is
            devoted to creating value by bringing you sophisticated, modern and,
            beautiful homes/properties with cautiously mapped-out and functional
            designs to suit your lifestyle.
            <br />
            With proactive industry leading brokers and agents, the SENA HOMES
            team provides high-quality service delivery and maximum value for
            money in a competitive property market. Our expertise combined with
            professionalism and strategic alliances facilitates a world-class
            service delivery that permits us to promptly exceed our clients’
            expectations.
          </p>
        </div>
      </v-container>
    </section>
    <section>
      <core-values-team></core-values-team>
    </section>
    <FindBestRE />
    <MobileApp />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
/* pages animation  */

#about {
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

#aboutHeader {
  background: linear-gradient(
      93deg,
      rgba(28, 33, 43, 0.7) 0%,
      rgba(28, 33, 43, 0.7) 20%
    ),
    url("/images/pngs/aboutHeader.png");
  background-size: cover;
  width: 100%;
  min-height: 40rem;
  margin-top: -96px;
}

.aboutHeader {
  height: 100%;
  min-height: 40rem;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}

.aboutHeader header {
  color: #fff;
  font-size: 5.4rem;
  font-weight: 700;
  margin-top: 90px;
  margin-bottom: 24px;
}

.aboutHeader p {
  font-weight: 400;
  font-size: 1.8rem;
  color: #fff;
  width: 60%;
  margin: 0 auto;
  mix-blend-mode: normal;
  opacity: 0.7;
}

#choice {
  padding: 97px 0 89px;
  background: linear-gradient(
      90deg,
      rgba(28, 33, 43, 0.83) 45.03%,
      rgba(28, 33, 43, 0) 96.53%
    ),
    url("/images/pngs/whySena.png");
  background-size: cover !important;
  text-align: center;
}

.contentChoice {
  display: flex;
  justify-content: center;
  flex-direction: column;

  p.goldText {
    font-weight: 500;
    text-transform: uppercase;
    color: var(--primary-color);
    font-size: 1.8rem;
    margin-bottom: 8px;
  }

  header {
    font-size: 4rem;
    font-weight: 700;
    color: #fff;
    margin-bottom: 50px;
  }

  p.content {
    width: 80%;
    margin: 0 auto;
    color: #fff;
    font-size: 1.8rem;
    font-weight: 500;
  }
}
@media (max-width: 390px) {
  p.content {
    width: 100% !important;
  }
}
</style>