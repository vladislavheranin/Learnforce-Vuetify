<template>
  <v-col lg="6" xl="6" md="12" sm="12" cols="12" class="pa-0 card-container">
    <v-card
        class="rounded-0 card-container__content"
        color="white"
        elevation="0"
    >
      <h3 class="font-weight-black mb-16 black--text local-title">
        {{ title }}
      </h3>

      <h4 class="font-weight-light mb-16 black--text">
        {{ subTitle }}
      </h4>

      <template v-if="type">
        <h6 v-if="type === 'signature'" class="font-weight-light mb-16 black--text">
          <span class="font-weight-bold">Angelien Landstra</span> – Founder Leadership Solutions
        </h6>
        <gefeliciteerd-modal v-if="type === 'btn'"></gefeliciteerd-modal>
      </template>
    </v-card>
  </v-col>
</template>

<script>

import GefeliciteerdModal from "@/components/modals/GefeliciteerdModal";
export default {
  name: "ContentHalfItem",
  props: {
    title: {
      type: String,
      default: '',
    },
    subTitle: {
      type: String,
      default: '',
    },
    type: {
      default: null,
    },
  },
  components: {
    GefeliciteerdModal,
  },
}
</script>

<style scoped>
.local-title {
  font-family: Neuton;
  font-size: 70px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-align: left;
  color: #011014;
}
</style>
