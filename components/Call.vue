<template>
  <div class="call">
    <div class="container">
      <div class="call-wrapper">
        <div class="call-img">
          <img src="@/assets/images/call-img.png" alt="" />
        </div>
        <form class="call-back">
          <div class="call-title">
            <h3>Закажите обратный звонок на консультацию</h3>
            <h4>Наши специалисты свяжутся с вами в течении нескольких минут</h4>
          </div>
          <label class="full">
            <input type="text" placeholder="Ваше имя" />
          </label>
          <label class="full">
            <input type="tel" placeholder="Ваш телефон" />
          </label>
          <label class="call-check" for="7">
            <input type="checkbox" name="check" id="7" />
            <span>Соглашаюсь на обработку персональных данных</span>
          </label>
          <div class="call-btn">
            <button type="submit">
              <span>Заказать звонок</span>
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
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.call {
  background: #f1eee7;

  &-wrapper {
    display: flex;
    justify-content: space-between;
  }

  .call-img{
    img{
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }

  .call-back {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    width: 35%;

    .full {
      width: 100%;
      input {
        width: 100%;
        margin-bottom: 20px;
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
  }
  .call-title {
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #3a3a3a;
      text-align: start;
      margin-bottom: 40px;
    }

    h4 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #3a3a3a;
      margin-bottom: 20px;
    }
  }

  .call-check {
    margin-bottom: 50px;
  }

  &-btn {
    button {
      display: flex;
      align-items: center;
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 19px;
      color: #909e80;
      border: none;
      border: 1px solid #909e80;
      background: transparent;
      padding: 15px;
      border-radius: 50px;
      cursor: pointer;

      &:hover {
        color: #f1eee7;
        background: #909e80;

        svg{
          fill: #f1eee7;
        }
      }
    }
  }
}
</style>
