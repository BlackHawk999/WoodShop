<template>
  <div class="goods-card">
    <h5>{{ title }}</h5>
    <div class="img-wrapper">
      <img :src="ImgUrl" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "GoodsCard",
  props: {
    title: {
      type: String,
    },
    ImgUrl: {
      type: String,
    },
  },
};
</script>

<style lang="scss" scoped>
.goods-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  cursor: pointer;

  &:hover {
    .img-wrapper {
      transform: scale(1.1);
    }
  }

  .img-wrapper {
    width: 320px;
    height: 320px;
    transition: 0.3s ease;

    img {
      width: 100%;
      height: 100%;
    }
  }

  h5 {
    font-family: Mont;
    font-style: normal;
    font-weight: 600;
    font-size: 34px;
    line-height: 44px;
    color: #3a3a3a;
  }
}
</style>
