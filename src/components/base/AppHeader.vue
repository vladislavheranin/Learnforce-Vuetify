<template>
  <v-app-bar
      height="90"
      app
      dark
      flat
      color="#141414"
      class="app-bar"
  >
    <div class="d-flex flex-column text-uppercase">
      <h3 class="font-weight-black text-left">Leadership</h3>
      <h3 class="font-weight-light text-left">Solutions</h3>
    </div>

    <v-spacer></v-spacer>

    <div class="d-flex align-center">
      <h3 class="font-weight-black text-left text-uppercase pr-10">Marcel</h3>
      <v-avatar
          color="white"
          size="57"
      ></v-avatar>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  name: "AppHeader"
}
</script>

<style scoped>

</style>
