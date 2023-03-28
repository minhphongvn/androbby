<template>
  <div>
    <div class="text-h4">Home</div>
    <div class="text-body-1">This is the home page</div>
    <v-btn class="mt-4" color="primary" depressed @click="toAbout">About</v-btn>
  </div>
</template>

<script lang="ts">
export default {
  name: "HomePage",
  data: () => ({
    //
  }),
  methods: {
    toAbout() {
      this.$router.push({
        name: "About",
        params: {
          value: "Data from Home",
        },
      });
    },
  },
};
</script>

<style>
</style>