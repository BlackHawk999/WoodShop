<template>
  <div class="contacts">
    <div class="container">
      <div class="contacts-wrapper">
        <div class="contacts-items">
          <div class="logo-wrapper">
            <img src="@/assets/images/Logo.png" alt="" />
          </div>
          <div class="adress">
            <h6>Производство и офис:</h6>
            <p>
              Россия, Московская область, д. Новосельцево, ул. Центральная, д.
              97 (15 км от МКАД)
            </p>
          </div>
        </div>
        <div class="contacts-links">
          <div class="links">
            <a href="#">Главная</a>
            <a href="#">Каталог</a>
            <a href="#">Расчет стоимости</a>
            <a href="#">Преимущества</a>
            <div class="privacy">
              <p>Политика конфиденциальности</p>
            </div>
          </div>
          <div class="links">
            <a href="#">Сотрудники</a>
            <a href="#">Отзывы</a>
            <a href="#">О нас</a>
            <a href="#">Контакты</a>
            <div class="email">
              <a href="mailto:elsadulaev@gmail.com">elsadulaev@gmail.com</a>
            </div>
          </div>
          <div class="telephone">
            <div class="tel">
              <p>Многоканальный</p>
              <a href="tel:+8 (495) 134-04-01">8 (495) 134-04-01</a>
            </div>
            <div class="tel-btn">
              <button>
                <span> Заказать обратный звонок </span>
                <svg
                  width="22"
                  height="22"
                  viewBox="0 0 22 22"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M13.7002 3.4375C14.8657 3.75095 15.9283 4.36513 16.7817 5.21853C17.6351 6.07193 18.2493 7.13459 18.5628 8.30007"
                    stroke="#909E80"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M12.9883 6.09448C13.6876 6.28255 14.3252 6.65106 14.8372 7.1631C15.3492 7.67514 15.7178 8.31274 15.9058 9.01203"
                    stroke="#909E80"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M7.94718 10.7264C8.66032 12.1843 9.84213 13.3608 11.3033 14.0673C11.4102 14.1179 11.5285 14.1399 11.6465 14.1309C11.7644 14.122 11.878 14.0825 11.9761 14.0164L14.1276 12.5817C14.2228 12.5182 14.3322 12.4795 14.4461 12.4691C14.56 12.4586 14.6747 12.4767 14.7798 12.5218L18.8049 14.2468C18.9416 14.3049 19.0558 14.4058 19.1302 14.5344C19.2045 14.663 19.2351 14.8123 19.2173 14.9598C19.09 15.9553 18.6043 16.8703 17.851 17.5335C17.0978 18.1966 16.1286 18.5625 15.125 18.5626C12.0253 18.5626 9.05252 17.3312 6.86069 15.1394C4.66886 12.9475 3.4375 9.97477 3.4375 6.87505C3.43755 5.87145 3.80342 4.90228 4.46659 4.14901C5.12975 3.39574 6.04475 2.91002 7.04026 2.7828C7.18774 2.76495 7.33703 2.79551 7.46562 2.86989C7.59422 2.94426 7.69517 3.05841 7.75325 3.19514L9.47978 7.22371C9.52444 7.32791 9.54264 7.44154 9.53275 7.55448C9.52287 7.66742 9.4852 7.77616 9.42312 7.87101L7.99343 10.0555C7.92836 10.1538 7.88989 10.2673 7.88179 10.3848C7.87368 10.5024 7.89621 10.6201 7.94718 10.7264V10.7264Z"
                    stroke="#909E80"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
              <div class="name">
                <p>© ООО «ВЛК», 2021</p>
              </div>
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
.contacts {
  background: #3a3a3a;
  position: relative;
  padding: 70px 0;

  &-items {
    display: flex;
    align-items: center;

    .logo-wrapper {
      margin-right: 35px;
    }

    .adress {
      display: flex;
      flex-direction: column;
      h6 {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 20px;
        line-height: 34px;
        color: #f1eee7;
        margin-bottom: 20px;
      }

      p {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 18px;
        line-height: 32px;
        color: #f1eee7;
      }
    }
  }

  &-links {
    display: flex;
    justify-content: space-between;
    background: #f1eee7;
    padding: 70px;
    bottom: 0%;
    right: 0;
    position: absolute;
    .links {
      display: flex;
      flex-direction: column;
      padding: 30px;

      a {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 15px;
        line-height: 19px;
        color: #3a3a3a;
        text-decoration: none;
        margin-bottom: 10px;

        &:hover {
          color: #9c9c9c;
        }
      }
    }

    .telephone {
      display: flex;
      flex-direction: column;
    }
    .tel {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      p {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 12px;
        line-height: 15px;
        color: #9c9c9c;
      }

      a {
        text-decoration: none;
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 34px;
        line-height: 44px;
        color: #909e80;
      }
    }

    .tel-btn {
      margin-top: 15px;
      button {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 15px;
        line-height: 19px;
        display: flex;
        align-items: center;
        text-align: center;
        color: #909e80;
        background: transparent;
        padding: 15px;
        border: none;
        border: 1px solid #909e80;
        border-radius: 50px;
        margin-bottom: 23px;
        transition: 0.3s all;


        &:hover {
          color: #f1eee7;
          background: #909e80;

          svg {
            fill: #f1eee7;
          }
        }
      }

      span {
        margin-right: 10px;
      }
    }
    .name {
      p {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 12px;
        line-height: 15px;
        color: #3a3a3a;
      }
    }
  }
}
</style>
