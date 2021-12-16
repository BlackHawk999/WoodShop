<template>
  <div class="employers">
    <div class="container">
      <div class="employers-wrapper">
        <div class="employers-title">
          <h3>Сотрудники нашей компании</h3>
          <h4>
            Рост и высокое качество продукции мы обеспечиваем за счет
            модернизации процесса производства, внедрения современных
            технологий, а также профессионализма сотрудников предприятия.
          </h4>
        </div>
        <div class="e-card-wrapper">
          <EmployersCard
            v-for="(e, i) in employers"
            :key="i"
            :img-url="e.imgUrl"
            :type="e.type"
            :title="e.title"
            :text="e.text"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import EmployersCard from "@/components/employ/EmployersCard.vue";
export default {
  name: "Employers",
  components: {
    EmployersCard,
  },
  data() {
    return {
      employers: [
        {
          type: "Отдел продаж",
          imgUrl: require("@/assets/images/employer.png"),
          title: "Манякин Вячеслав Семенович",
          text: "Менеджер по продажам",
        },
        {
          type: "Производство",
          imgUrl: require("@/assets/images/employer-2.png"),
          title: "Суснинаслава Борисовна",
          text: "Менеджер по продажам",
        },
        {
          type: "Руководство",
          imgUrl: require("@/assets/images/employer.png"),
          title: "Вольваков Георгий Алексеевич",
          text: "Менеджер по продажам",
        },
        {
          type: "Отдел продаж",
          imgUrl: require("@/assets/images/employer-2.png"),
          title: "Коренёва Алиса Василиевна",
          text: "Менеджер по продажам",
        },
        {
          type: "Производство",
          imgUrl: require("@/assets/images/employer.png"),
          title: "Мосин Федор Ростиславович",
          text: "Менеджер по продажам",
        },
        {
          type: "Менежер продаж",
          imgUrl: require("@/assets/images/employer-2.png"),
          title: "Фомичева Ульяна Карповна",
          text: "Менеджер по продажам",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.employers {
  background: #ffffff;
  padding: 70px 0;
  &-title {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 70px;

    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #3a3a3a;
      width: 25%;
    }

    h4 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #3a3a3a;
      width: 42%;
    }
  }

  .e-card-wrapper{
    display: grid;
    grid-template-columns: repeat(3,1fr);
    row-gap: 0;
  }
}
</style>
