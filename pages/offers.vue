<template>
  <div>
    <Header />
    <hr />
    <div class="offer_page">
      <Card />
      <Card />
    </div>
    <!-- <div class="tabs"></div>
    <tabs>
      <tab active="true" label="tab1">
        <p>11111111111111111</p>
      </tab>
      <tab label="tab2">
        <p>2222222222222222</p>
      </tab>
      <tab label="tab3">
        <p>3333333333333</p>
      </tab>
    </tabs> -->
  </div>
</template>

<script>
import Header from "@/components/common/TheHeader";
import Card from "@/components/common/Card";
// import Tabs from "@/components/common/Tabs;
// import Tab from "@/components/common/Tab;

export default {
  name: "offers",
  components: { Header, Card },
  head: {
    title: "Предложения",
  },
  data() {
    return {
      a: [],
    };
  },
};
</script>

<style lang="scss" scoped>
.offer_page {
  display: flex;
}
@media (max-width: 1024px) {
  .offer_page {
    flex-direction: column;
    align-items: center;
  }
}
</style>
