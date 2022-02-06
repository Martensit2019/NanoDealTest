<template>
  <div>
    <h1>Dashboard</h1>
    <tabs>
      <tab name="Активные" image="actives.svg" :selected="true">
        <Card />
      </tab>
      <tab name="На модерации" image="actives">
        <h1>На модерации</h1>
      </tab>
      <tab name="Черновики" image="actives">
        <h1>Черновики</h1>
      </tab>
      <tab name="Архив" image="actives">
        <h1>Архив</h1>
      </tab>
    </tabs>
  </div>
</template>

<script>
import Card from "@/components/common/Card";
import Tabs from "@/components/common/Tabs";
import Tab from "@/components/common/Tab";
export default {
  name: "index",
  components: { Card, Tabs, Tab },
  head: {
    title: "Dashboard",
  },
};
</script>
