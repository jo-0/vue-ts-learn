<script setup lang="ts">
import ConfigForm from "./components/ConfigForm.vue";
</script>

<template>
  <div class="container is-fluid">
    <header>
      <h1 class="title">App name</h1>
    </header>
    <config-form />
  </div>
</template>

<style scoped lang="scss">
.container {
  padding-left: 64px;
  padding-right: 64px;
}

.title {
  padding: 10px 10px;
  text-align: center;
}
</style>
