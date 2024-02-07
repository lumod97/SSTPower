<template>
  <div id="app">
    <dashboard-view></dashboard-view>
  </div>
</template>

<script>
import DashboardView from '@/components/DashboardView.vue';

export default {
  name: 'App',
  components: {
    DashboardView
  }
}
</script>

<style>

.cursor-pointer{
  cursor: pointer;
}
</style>
