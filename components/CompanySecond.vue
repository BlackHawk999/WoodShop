<template>
  <div class="company-second">
    <div class="container">
      <div class="company-part-wrapper">
        <div class="company-part-img">
          <img src="@/assets/images/company-2.png" alt="" />
        </div>
        <div class="company-second-titles">
          <h4>
            Мы работаем только с зимним лесом, который обрабатывается на наших
            станках европейского стандарта.
          </h4>
          <p>
            Каждая доска изготавливается из спелого леса нашей собственной
            лесозаготовки и проходит ручной отбор, что позволяет выдерживать
            высшее качество наших материалов.
          </p>
          <p>
            Благодаря собственному производству, лесозаготовке и складам, мы
            обеспечиваем своим клиентам лучшие цены и быстрое выполнение
            заказов. Поэтому прийдя к нам один раз - клиент остается навсегда.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.company-second {
  background: #a2b192;

  .company-part-wrapper {
    display: flex;
    justify-content: flex-end;
  }

  .company-part-img{
    display: flex;
    justify-content: flex-start;
    width: 70%;
    transform: translateX(-3%);
  }

  .company-second-titles {
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 60%;

    h4 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 34px;
      line-height: 44px;
      color: #f1eee7;
      margin-bottom: 50px;
    }

    p {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #f1eee7;
      margin-bottom: 30px;
    }
  }
}
</style>
