<template>
  <div>
    <div class="text-h4">About</div>
    <div class="text-body-1">
      {{ info }}
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "AboutPage",
  data: () => ({
    info: "This is the about page",
  }),
  created() {
    this.info = this.$route.params.value;
  },
};
</script>

<style>
</style>