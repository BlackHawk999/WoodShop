<template>
  <div class="goods">
    <div class="container">
      <div class="goods-wrapper">
        <div class="goods-title">
          <h3>Лучшие материалы под ваши потребности</h3>
          <h4>
            Наша компания работает с 2000 года. Мы – не просто торговый
            посредник, а производитель. Поэтому предлагаем материалы наилучшего
            качества под любой запрос.
          </h4>
        </div>
        <div class="goods-items">
          <GoodsCard
            v-for="(g, i) in goods"
            :key="i"
            :title="g.title"
            :img-url="g.imgUrl"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import GoodsCard from "@/components/goods/GoodsCard.vue";
export default {
  name: "Goods",
  components: {
    GoodsCard,
  },

  data() {
    return {
      goods: [
        {
          title: "Обрезная доска",
          imgUrl: require("@/assets/images/doska-obrez-1.png"),
        },
        {
          title: "Обрезной брус",
          imgUrl: require("@/assets/images/doska-obrez-2.png"),
        },
        {
          title: "Евровагонка",
          imgUrl: require("@/assets/images/doska-obrez-3.png"),
        },
        {
          title: "Строганная доска",
          imgUrl: require("@/assets/images/doska-obrez-4.png"),
        },
        {
          title: "Строганный брус",
          imgUrl: require("@/assets/images/doska-obrez-5.png"),
        },
        {
          title: "Вагонка штиль",
          imgUrl: require("@/assets/images/doska-obrez-6.png"),
        },
        {
          title: "Имитация бруса",
          imgUrl: require("@/assets/images/doska-obrez-7.png"),
        },
        {
          title: "Блок-хаус",
          imgUrl: require("@/assets/images/doska-obrez-8.png"),
        },
        {
          title: "Вагонка четверть",
          imgUrl: require("@/assets/images/doska-obrez-9.png"),
        },
        {
          title: "Планкен прямой",
          imgUrl: require("@/assets/images/doska-obrez-10.png"),
        },
        {
          title: "Планкен скошенный ",
          imgUrl: require("@/assets/images/doska-obrez-11.png"),
        },
        {
          title: "Доска пола",
          imgUrl: require("@/assets/images/doska-obrez-12.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.goods {
  background: #ffffff;
  padding: 75px 0;

  &-title {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 100px;
    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #3a3a3a;
      width: 32%;
    }

    h4 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #3a3a3a;
      width: 40%;
    }
  }

  &-items {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 40px;

    .goods-card {
      
      &:not(:nth-child(3n)) {
        border-right: 1px solid grey;
      }
    }
  }
}
</style>
