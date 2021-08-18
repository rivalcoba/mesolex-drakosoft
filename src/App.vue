<template>
  <div id="app">
    <navigation-bar />
    <div class="breacrumbs">
      <h1>Breadcrumbs</h1>
    </div>
    <router-view />
  </div>
</template>
<script>
import NavigationBar from '@/components/NavigationBar.vue';

export default {
  components: {
    NavigationBar,
  },
};
</script>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 10px;
}
</style>
