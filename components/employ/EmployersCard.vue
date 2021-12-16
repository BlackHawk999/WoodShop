<template>
  <div class="employer">
    <img :src="imgUrl" alt="" />
    <div class="employer-info">
      <div class="type-btn">
        <button>{{ type }}</button>
      </div>
      <h5>{{ title }}</h5>
      <h6>{{ text }}</h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "EmployersCard",
  props: {
    imgUrl: {
      type: String,
    },
    type: {
      type: String,
    },
    title: {
      type: String,
    },
    text: {
      type: String,
    },
  },
};
</script>

<style lang="scss" scoped>
.employer {
  position: relative;

  &:hover {
    img {
      transition: 0.5s ease;
      opacity: 0;
    }

    .employer-info {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      position: absolute;
      top: 40%;
      right: 0%;
      width: 100%;

      h5 {
        font-family: Mont;
        font-style: normal;
        font-weight: 600;
        font-size: 34px;
        line-height: 44px;
        color: #3a3a3a;
        margin: 65px 0 35px 0;
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
    .type-btn {
      display: block;
    }
  }

  &-info {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    position: absolute;
    top: 60%;
    right: 10%;
    width: 70%;

    .type-btn {
      display: none;

      button {
        display: none;
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
        border: none;
        border: 1px solid #909e80;
        border-radius: 50px;
        padding: 8px 20px;
      }
    }

    h5 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 34px;
      line-height: 44px;
      color: #ffffff;
      margin: 65px 0 35px 0;
    }

    h6 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 20px;
      line-height: 34px;
      color: #ffffff;
    }
  }
}
</style>
