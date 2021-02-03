<template>
  <v-footer
      color="#141414"
      padless
  >
    <v-card
        flat
        tile
        width="100%"
        color="#141414"
        class="text-center"
    >
      <v-card-text class="white--text">
        <v-col color="white" cols="12" class="d-flex flex-column text-uppercase text-center">
          <h3 class="font-weight-black white-text leadership">Leadership</h3>
          <h3 class="font-weight-light white-text solutions">Solutions</h3>
        </v-col>
      </v-card-text>
      <v-card-text class="mb-7">
        <v-btn
            v-for="icon in icons"
            :key="icon"
            icon
            color="white"
            class="mx-2"
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>

      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  name: "AppFooter",
  data() {
    return {
      icons: [
        'mdi-linkedin',
        'mdi-youtube',
        'mdi-facebook',
      ],
    }
  },
}
</script>

<style scoped>

</style>
