<template>
  <div class="wrapper">
    <div class="container">
      <div class="mobile-head">
        <div class="mobile-head__menu">
          <img src="@/assets/images/icons/nav/menu-mob.svg" />
        </div>
        <Logo />
        <div class="mobile-head__avatar">
          <img src="@/assets/images/avatar.jpg" />
        </div>
      </div>
      <div class="wrapper__inner">
        <aside class="aside">
          <Logo />
          <Navigation />
        </aside>
        <div class="main">
          <Nuxt />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Logo from "@/components/common/Logo";
import Navigation from "@/components/common/Navigation";
export default {
  components: { Logo, Navigation },
};
</script>

<style lang="scss" scoped>
@media (max-width: 764px) {
  .aside {
    display: none;
  }
}
</style>
