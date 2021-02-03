<template>
  <v-col cols="6" class="pa-0 images">
    <v-card class="rounded-0">
      <v-img
          :src="imgLink"
          class="white--text align-end"
          gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
          height="960px"
      >
      </v-img>
    </v-card>
  </v-col>
</template>

<script>
export default {
  name: "PhotoItem",
  props: {
    imgLink: {
      type: String,
      default: '',
    }
  }
}

</script>

<style scoped>

@media (max-width: 1400px) {
  .images {
    display: none;
  }
}

</style>
