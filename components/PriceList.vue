<template>
  <div class="price-list">
    <div class="container">
      <div class="price-wrapper">
        <!-- <div class="price-list-second-wrapper"> -->
        <form class="price-form">
          <div class="price-list-title">
            <h3>Прайс-лист за считанные секунды</h3>
          </div>
          <label class="sort">
            <input type="text" name="" id="" placeholder="Ваше имя" />
          </label>
          <label class="sort">
            <input type="tel" name="" id="" placeholder="Ваш телефон" />
          </label>
          <label class="sort">
            <input type="email" name="" id="" placeholder="Ваш e-mail" />
          </label>
          <div class="check">
            <input type="checkbox" />
            <span>Соглашаюсь на обработку персональных данных</span>
          </div>
          <div class="file-send">
            <button type="submit">
              <span>Получить прайс</span>
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
            <div class="file-size">
              <p>Файл PDF</p>
              <h6>3.5МБ</h6>
            </div>
          </div>
        </form>
        <div class="price-list-img">
          <img src="@/assets/images/price-list-img.png" alt="" />
        </div>
      </div>
      <!-- </div> -->
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.price-list {
  background: #f1eee7;
  .price-list-title {
    margin-bottom: 35px;
    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #3a3a3a;
    }
  }
  .price-wrapper {
    display: flex;
    justify-content: space-between;
  }
  .price-form {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    width: 30%;

    .sort {
      width: 100%;

      input {
        width: 100%;
        margin-bottom: 35px;
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
      margin-right: 25px;
      transition: 0.3s all;

      &:hover {
        color: #f1eee7;
        background: #909e80;

        svg {
          fill: #f1eee7;
        }
      }
    }

    .check {
      margin: 30px 0 50px 0;
    }

    .file-send {
      display: flex;
      align-items: center;
    }

    .file-size {
      display: flex;
      flex-direction: column;

      p {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 12px;
        line-height: 15px;
        color: #9c9c9c;
      }

      h6 {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 20px;
        line-height: 34px;
        color: #3a3a3a;
      }
    }
  }

  .price-list-img {
    width: 50%;

    img{
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
}
</style>
