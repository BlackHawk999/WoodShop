<template>
  <div class="header">
    <Navbar />
    <div class="container">
      <div class="main-wrapper">
        <div class="titles-wrapper">
          <div class="header-title">
            <h1>Волоколамский</h1>
            <h2>Лесоперерабатывающий Комплекс</h2>
            <div class="header-sub-title">
              <div class="year-wrapper">
                <h3 class="year">
                  20
                  <p>лет</p>
                </h3>
                <h4>опыт работы</h4>
              </div>
              <div class="branch-wrapper">
                <h3 class="branch">
                  10
                  <p>филиалов</p>
                </h3>
                <h4>в регионах РФ</h4>
              </div>
              <div class="clients-wrapper">
                <h3 class="clients">
                  9000
                  <p>клиентов</p>
                </h3>
                <h4>более 30 000 заказов</h4>
              </div>
            </div>
          </div>
          <div class="header-price-info">
            <h5>
              Ручная сортировка досок, только спелый лес. На сегодняшний день
              это лучшее предложение на рынке России
            </h5>
            <div class="price-btn">
              <button>
                <span> Получить прайс </span>
                <svg
                  width="29"
                  height="22"
                  viewBox="0 0 29 22"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1 11L25 11"
                    stroke="#A2B192"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M19.375 4.8125L25.5625 11L19.375 17.1875"
                    stroke="#A2B192"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
export default {
  name: "Header",
  components: {
    Navbar,
  },
};
</script>

<style lang="scss" scoped>
.header {
  min-height: 100vh;
  background: url("../assets/images/background-2.jpg");
  position: relative;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;

  &::before {
    content: "";
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    left: 0;
    background: linear-gradient(
      355.26deg,
      rgba(19, 16, 15, 0.74) 43.78%,
      rgba(31, 26, 25, 0) 95.28%
    );
    z-index: 1;
  }

  .main-wrapper {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
  }

  .titles-wrapper {
    display: flex;
    justify-content: space-between;
    width: 100%;
    height: 100%;
    z-index: 2;
  }

  &-title {
    display: flex;
    flex-direction: column;
    width: 50%;

    h1 {
      font-weight: 600;
      font-size: 100px;
      line-height: 62px;
      color: #f1eee7;
      margin: 0;
      margin-bottom: 25px;
    }

    h2 {
      font-weight: 600;
      font-size: 52px;
      line-height: 62px;
      color: #f1eee7;
      margin: 0;
      margin-bottom: 30px;
    }
  }

  &-sub-title {
    display: flex;
    align-items: center;
    justify-content: space-between;

    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 800;
      font-size: 126px;
      line-height: 161px;
      color: #a2b192;
      margin: 0;
    }

    p {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 16px;
      color: #a2b192;
    }

    h4 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #f1eee7;
      margin: 0;
    }

    .year-wrapper {
      position: relative;

      p {
        position: absolute;
        top: 0;
        right: -20px;
      }
    }
    .branch-wrapper {
      position: relative;

      p {
        position: absolute;
        top: 0;
        right: -50px;
      }
    }
    .clients-wrapper {
      position: relative;

      p {
        position: absolute;
        top: 0;
        right: -65px;
      }
    }
  }

  .header-price-info {
    display: flex;
    flex-direction: column;
    width: 25%;
    position: relative;

    h5 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #f1eee7;
      margin: 0;
      margin-bottom: 60px;
    }

    button {
      color: #a2b192;
      background: transparent;
      border: 1px solid #a2b192;
      box-sizing: border-box;
      border-radius: 41px;
      padding: 15px 35px 15px 25px;
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 19px;
      text-align: center;
      cursor: pointer;
      position: relative;
      overflow: hidden;
      display: flex;
      align-items: center;

      &:after {
        background: #fff;
        content: "";
        height: 155px;
        left: -75px;
        opacity: 0.2;
        position: absolute;
        top: -50px;
        transform: rotate(35deg);
        transition: all 550ms cubic-bezier(0.19, 0.7, 0.22, 1);
        width: 50px;
        z-index: 10;
      }

      &:hover {
        &:after {
          left: 120%;
          transition: all 550ms cubic-bezier(0.19, 1, 0.22, 1);
        }
      }

      span {
        margin-right: 20px;
      }
    }
  }

  .main-img {
    bottom: 0;
    left: 0;
    right: 0;

    img {
      width: 100%;
      height: 100%;
    }
  }
}
</style>
