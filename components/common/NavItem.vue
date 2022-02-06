<template>
  <NuxtLink class="nav-item" :to="link">
    <div class="nav-item__img" v-html="icon">
      <!-- <img :src="icon" alt="" /> -->
      <!-- {{ v-html=icon}} -->
    </div>
    {{ label }}
  </NuxtLink>
</template>

<script>
export default {
  name: "NavItem",
  props: {
    label: {
      type: String,
      required: true,
    },
    icon: {
      type: String,
      required: "",
    },
    link: {
      type: String,
      required: false,
      default: "",
    },
  },
};
</script>
