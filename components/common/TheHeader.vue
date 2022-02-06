<template>
  <header class="header">
    <div class="header__title">Предложения</div>

    <div class="search-box">
      <div class="search-box__img">
        <img src="@/assets/images/icons/search.svg" />
      </div>

      <input class="search-box__input" type="text" placeholder="Поиск" />
    </div>
    <div class="avatar">
      <img src="@/assets/images/avatar.jpg" />
    </div>
  </header>
</template>

<style lang="scss" scoped>
@media (max-width: 764px) {
  .avatar {
    display: none;
  }
}
</style>
