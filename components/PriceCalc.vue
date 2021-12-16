<template>
  <div class="price-calc">
    <div class="container">
      <div class="wrapper-price">
        <div class="price-first">
          <div class="price-title">
            <h3>Рассчитаем стоимость нужного материала</h3>
          </div>
          <form class="price-form">
            <label class="sort">
              <input type="text" name="" id="" placeholder="Ваше имя" />
            </label>
            <label class="sort">
              <input type="tel" name="" id="" placeholder="Ваш телефон" />
            </label>
            <label class="sort">
              <input type="email" name="" id="" placeholder="Ваш e-mail" />
            </label>
            <label class="sort">
              <input type="text" placeholder="Сообщение" />
            </label>
            <div class="check">
              <label for="55">
                <input type="checkbox" id="55" />
                <span>Соглашаюсь на обработку персональных данных</span>
              </label>
            </div>
            <button type="submit">
              <span>Отправить</span>
              <svg
                width="31"
                height="22"
                viewBox="0 0 31 22"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M3 11L27 11"
                  stroke="#909E80"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
                <path
                  d="M21.375 4.8125L27.5625 11L21.375 17.1875"
                  stroke="#909E80"
                  stroke-width="1.5"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </button>
          </form>
        </div>
        <div class="price-photo">
          <div class="photo-wrapper">
            <img src="@/assets/images/price-photo.png" alt="" />
          </div>
          <div class="sort-wrapper">
            <div class="wood-sort">
              <div class="material">
                <h5>Материал</h5>
                <input type="text" name="" id="" placeholder="Название" />
              </div>
              <div class="wood-size">
                <h5>Параметры</h5>
                <input type="text" placeholder="Толщина, мм" />
                <input type="text" placeholder="Ширина, мм" />
                <input type="text" placeholder="Длина, м" />
              </div>
            </div>
            <div class="wood-category">
              <div class="sort-wrp">
                <label for="1" class="sort">
                  <h5>Сорт</h5>
                  <input type="checkbox" name="wood" id="1" />
                  <span>Extra</span>
                  <input type="checkbox" name="wood" id="1" />
                  <span>AB</span>
                </label>
              </div>
              <label for="2">
                <h5>Браширование</h5>
                <input type="checkbox" id="2" />
                <span>Да, нужно</span>
              </label>
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
.price-calc {
  background: #eee8d8;

  .wrapper-price {
    display: flex;
    justify-content: space-between;
    position: relative;
  }

  .price-title {
    width: 60%;
    margin-bottom: 5px;
    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #3a3a3a;
    }
  }

  .price-first {
    width: 30%;
  }

  .price-form {
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    .sort {
      width: 100%;

      input {
        width: 100%;
        margin-bottom: 15px;
      }
    }

    input {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 34px;
      color: #9c9c9c;
      background: transparent;
      outline: none;
      border: none;
      border-bottom: 1px solid #909e80;
    }
    .check {
      display: flex;
      align-items: center;
      margin-top: 60px;
      margin-bottom: 50px;

      input {
        margin-right: 10px;
      }
    }

    button {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 19px;
      color: #909e80;
      display: flex;
      align-items: center;
      padding: 15px;
      border: none;
      border: 1px solid #909e80;
      border-radius: 41px;
      background: transparent;
      cursor: pointer;
      transition: 0.3s all;

      &:hover {
        color: #f1eee7;
        background: #909e80;

        svg {
          fill: #f1eee7;
        }
      }
      span {
        margin-right: 15px;
      }
    }
  }

  .price-photo {
    
    .photo-wrapper {
      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
    .sort-wrapper {
      display: flex;
      background: #3a3a3a;
      padding: 130px 70px;
      position: absolute;
      top: 30%;
      right: 0;

      h5 {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 34px;
        line-height: 44px;
        color: #f1eee7;
      }
      input {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 15px;
        line-height: 34px;
        color: #9c9c9c;
        background: transparent;
        outline: none;
        border: none;
        border-bottom: 1px solid #909e80;
      }

      .wood-sort {
        padding: 35px;
        .material {
          margin-bottom: 85px;
        }
      }

      .wood-category {
        padding: 35px;

        span {
          font-family: Mont;
          font-style: normal;
          font-weight: 600;
          font-size: 20px;
          line-height: 34px;
          color: #f1eee7;
          margin-right: 15px;
          margin-left: 15px;
        }

        .sort-wrp {
          margin-bottom: 85px;
        }
      }
    }
  }
}
</style>
