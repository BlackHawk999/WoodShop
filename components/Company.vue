<template>
  <div class="company">
    <div class="container">
      <div class="company-wrapper">
        <div class="company-first-info">
          <div class="first-info-title">
            <h3>О компании</h3>
            <h4>
              Мы находимся на российском рынке уже более 20 лет. За это время
              мы:
            </h4>
          </div>
          <div class="company-bckg-img">
            <img src="@/assets/images/company-bckg.png" alt="" />
          </div>
          <div class="company-main-img">
            <img src="@/assets/images/company-img.png" alt="" />
          </div>
        </div>
        <div class="company-second-info">
          <div class="company-infos">
            <div class="text">
              <h3>30 000</h3>
              <h6>Заказов выполнили</h6>
            </div>
          </div>
          <div class="company-infos middle">
            <div class="text more">
              <h3>
                9000
                <p>более</p>
              </h3>
              <h6>клиентов обслужили</h6>
            </div>
          </div>
          <div class="company-infos">
            <div class="text more">
              <h3>
                300
                <p>более</p>
              </h3>
              <h6>крупных компаний стали нашими постоянными клиентами</h6>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.company {
  position: relative;
  background: #3a3a3a;
  padding: 70px 0;

  &-wrapper {
    display: flex;
    justify-content: space-between;
  }

  .company-first-info {
    display: flex;
    flex-direction: column;
    width: 33%;
  }

  .first-info-title {
    display: flex;
    flex-direction: column;

    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #f1eee7;
      margin-bottom: 60px;
    }

    h4 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 40px;
      line-height: 56px;
      color: #f1eee7;
    }
  }

  .company-bckg-img {
    position: absolute;
    left: 10%;
    bottom: -45%;
  }
  .company-main-img {
    position: absolute;
    left: 0;
    bottom: -45%;
    z-index: 2;
  }

  .company-second-info {
    display: flex;
    flex-direction: column;
  }
  .company-infos {
    &.middle {
      border-top: 1px solid #a2b192;
      border-bottom: 1px solid #a2b192;
    }

    .text {
      margin: 60px 0;
      &.more {
        position: relative;

        h3 {
          text-align: center;
        }

        p {
          position: absolute;
          top: 17%;
          left: 0;
        }
      }
    }

    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 800;
      font-size: 126px;
      line-height: 161px;
      color: #a2b192;

      p {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 15px;
        line-height: 16px;
        color: #a2b192;
      }
    }

    h6 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #f1eee7;
    }
  }
}
</style>
