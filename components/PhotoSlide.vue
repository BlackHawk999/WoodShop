<template>
  <div class="photo-slide">
    <div class="container">
      <div class="photos-wrapper">
        <div class="photos-title">
          <h3>Фотографии производства</h3>
        </div>
        <VueSlickCarousel v-bind="settings">
          <div>
            <img
              class="photo-slide__img"
              src="@/assets/images/slide-6.png"
              alt=""
            />
          </div>
          <div>
            <img
              class="photo-slide__img"
              src="@/assets/images/slide-3.png"
              alt=""
            />
          </div>
          <div>
            <img
              class="photo-slide__img"
              src="@/assets/images/slide-3.png"
              alt=""
            />
          </div>
          <div>
            <img
              class="photo-slide__img"
              src="@/assets/images/slide-4.png"
              alt=""
            />
          </div>
          <div>
            <img
              class="photo-slide__img"
              src="@/assets/images/slide-5.png"
              alt=""
            />
          </div>
          <div>
            <img
              class="photo-slide__img"
              src="@/assets/images/slide-6.png"
              alt=""
            />
          </div>
        </VueSlickCarousel>
      </div>
    </div>
  </div>
</template>

<script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";

export default {
  name: "PhotoSlide",
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        centerPadding: "20px",
        focusOnSelect: true,
        infinite: true,
        slidesToShow: 3,
        speed: 500,
        autoplay: true,
        arrows: false,
      },
    };
  },
};
</script>

<style lang="scss" scoped>
.photo-slide {
  background: #a2b192;
  padding: 50px 0;

  &__img {
    width: 100%;
    pointer-events: none;
    cursor: pointer;
  }

  .photos-title {
    width: 75px;
    margin-bottom: 70px;
    h3 {
      font-family: Mont;
      font-style: normal;
      font-weight: 600;
      font-size: 52px;
      line-height: 66px;
      color: #f1eee7;
    }
  }
}
</style>
