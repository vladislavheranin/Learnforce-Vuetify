<template>
  <v-dialog
      v-model="dialog"
      width="757"
      hide-overlay
  >
    <template v-slot:activator="{ on, attrs }">
      <v-btn
          color="white"
          outlined
          plain
          raised
          v-bind="attrs"
          v-on="on"
          class="mb-16"
      > Download het eerste werkboek </v-btn>
    </template>

    <v-card height="864" class="modal">
      <v-card-text>
        <v-col cols="12" class="mb-0 text-center">
          <v-avatar height="119px" width="119px" class="mx-auto">
            <img
                src="https://cdn.vuetifyjs.com/images/cards/house.jpg"
                alt=""
            >
          </v-avatar>
        </v-col>
        <v-col cols="12" class="mb-13 horizontal-area">
          <p class="text-center font-weight-bold">Gefeliciteerd!</p>
        </v-col>
        <v-col cols="12" class="mt-3 horizontal-area horizontal-area_secondary">
          <p class="text-center">Je gaat aan de slag met het curriculum over:</p>
        </v-col>
        <v-col cols="12" class="mt-0 horizontal-area horizontal-area_low">
          <p class="text-center">Zelfleiderschap</p>
        </v-col>
        <v-col cols="12" class="mt-0 mb-0 horizontal-area horizontal-area_secondary">
          <p class="text-center">Je gaat aan de slag met het curriculum over:</p>
        </v-col>
        <v-col cols="12" class="mt-0 mb-0 horizontal-container">
          <gefeliciteerd-modal-person-item class="ml-16 mr-16"></gefeliciteerd-modal-person-item>
          <gefeliciteerd-modal-person-item class="ml-16 mr-16"></gefeliciteerd-modal-person-item>
          <gefeliciteerd-modal-person-item class="ml-16"></gefeliciteerd-modal-person-item>
        </v-col>
        <v-col cols="5" class="mx-auto">
          <button class="button">Verstuur</button>
        </v-col>
      </v-card-text>
    </v-card>
  </v-dialog>
</template>

<script>
import GefeliciteerdModalPersonItem from "@/components/modals/GefeliciteerdModalPersonItem";

export default {
  name: "GefeliciteerdModal",
  data() {
    return {
      dialog: false
    }
  },
  props: {
    color: {
      default: 'white',
    },
  },
  components: {
    GefeliciteerdModalPersonItem,
  },
}
</script>

<style scoped>

.modal {
  padding-bottom: 100px;
  padding-top: 50px;
}

.horizontal-area {
  font-size: 60px;
}

.horizontal-area_low {
  font-size: 30px;
}

.horizontal-area_secondary{
  font-family: Roboto;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.3;
  letter-spacing: normal;
  text-align: left;
  color: #a8a8a8;
}

.button {
  height: 70px;
  border-radius: 8px;
  border: solid 2px #0d0303;
  background-color: inherit;
  width: 100%;
  text-align: center;
  font-family: Roboto;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.3;
  letter-spacing: normal;
  color: #0d0303;
}

.horizontal-container {
  position: relative;
  overflow: hidden;
  height: 150px;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
}

</style>
