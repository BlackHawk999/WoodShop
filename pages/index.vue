<template>
  <div class="page">
    <Header />
    <Goods />
    <AboutUs />
    <PriceCalc />
    <PhotoSlide />
    <Employers />
    <Call />
    <FeedBacks />
    <PriceList />
    <Company />
    <CompanySecond />
    <Contacts />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Goods from "@/components/goods/Goods.vue";
import AboutUs from "@/components/AboutUs.vue";
import PriceCalc from "@/components/PriceCalc.vue";
import PhotoSlide from "@/components/PhotoSlide.vue";
import Employers from "@/components/employ/Employers.vue";
import Call from "@/components/Call.vue";
import FeedBacks from "@/components/FeedBacks.vue";
import PriceList from "@/components/PriceList.vue";
import Company from "@/components/Company.vue";
import CompanySecond from "@/components/CompanySecond.vue";
import Contacts from "@/components/Contacts.vue";

export default {
  name: "homePage",
  components: {
    Header,
    Goods,
    AboutUs,
    PriceCalc,
    PhotoSlide,
    Employers,
    Call,
    FeedBacks,
    PriceList,
    Company,
    CompanySecond,
    Contacts,
  }
};
</script>
