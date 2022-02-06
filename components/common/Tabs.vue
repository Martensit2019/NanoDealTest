<template>
  <div>
    <div class="tabs">
      <a
        v-for="tab in tabs"
        :class="{ 'is-active': tab.isActive }"
        class="tab__head"
        :href="tab.href"
        @click="selectTab(tab)"
      >
        <img :src="require('~/assets/images/icons/actives.svg')" />
        {{ tab.image }}</a
      >
    </div>
    <div class="tabs-details">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return { tabs: [] };
  },
  created() {
    this.tabs = this.$children;
  },
  methods: {
    selectTab(selectedTab) {
      this.tabs.forEach((tab) => {
        tab.isActive = tab.name == selectedTab.name;
      });
    },
  },
};
</script>
<style lang="scss" scoped>
.tab__head {
  display: inline-flex;
  align-items: center;
  padding: 10px 13px;  
  font-weight: 600;
  font-size: 14px;
  line-height: 16px;
  text-align: center;
  color: #2d3134;
  border-radius: 10px;
  margin-bottom: 30px;
  &.is-active{
    background-color: #fff;
  }
  & + .tab__head {
    margin-left: 18px;
  }
  img{
    margin-right: 10px;
  }
}
</style>
