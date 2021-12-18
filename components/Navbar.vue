<template>
  <div :class="['navbar', { active: isActive }]">
    <div class="logo">
      <img src="@/assets/images/Logo.png" alt="" />
      <div class="logo-title">
        <p>Волоколамский Лесоперерабатывающий Комплекс</p>
      </div>
    </div>
    <div class="navbar-links">
      <a href="#">Главная</a>
      <a href="#">Каталог</a>
      <a href="#">Расчет стоимости</a>
      <a href="#">Преимущества</a>
      <a href="#">Сотрудники</a>
      <a href="#">Отзывы</a>
      <a href="#">О нас</a>
      <a href="#">Контакты</a>
      <div class="navbar-tel">
        <a href="tel:+84951340401">
          +8 (495) 134-04-01
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    scrollFunc() {
      const scrollPos = document.documentElement.scrollTop;

      if (scrollPos > 0) {
        return (this.isActive = true);
      }

      this.isActive = false;
    },
  },
  mounted() {
    document.addEventListener("scroll", this.scrollFunc);
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 35px;
  position: fixed;
  z-index: 1000;
  top: 0;
  left: 0;
  right: 0;
  transition: 0.2s;

  &.active {
    background: white;

    .navbar-links {
      a {
        color: #3a3a3a;
        transition: all 0.5s;

        &:hover {
          color: #a3df22a6;
          transform: translateY(-10px);
        }
      }
    }
  }

  .logo {
    display: flex;
    align-items: center;

    img {
      margin-right: 20px;
    }

    p {
      width: 50%;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 20px;
      color: #f1eee7;
    }
  }

  &-links {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 50%;
    a {
      color: #f1eee7;
      text-decoration: none;
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 15px;
      line-height: 19px;
      transition: all 0.5s;

      &:hover {
        color: #a3df22a6;
        transform: translateY(-10px);
      }
    }
  }
  &-tel {
    display: flex;
    align-items: center;

    a {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 18px;
      line-height: 23px;
      color: #f1eee7;
      margin-right: 20px;
    }
  }
}
</style>
