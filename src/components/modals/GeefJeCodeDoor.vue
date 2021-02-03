<template>
  <v-dialog
      v-model="dialog"
      width="757"  
  >
    <template v-slot:activator="{ on, attrs }">
      <v-btn
          :color="color"
          outlined
          plain
          raised
          class="main-btn"
          x-large
          v-bind="attrs"
          v-on="on"
      >
        Geef je code door
      </v-btn>
    </template>

    <v-card class="modal">
      <v-card-text>
        <v-col cols="12" class="my-2 horizontal-area">
          <p class="font-weight-black black--text text-center">Geef je code door</p>
        </v-col>
        <v-col cols="12" class="horizontal-area horizontal-area_low">
          <p class="text-center">Om de content van de <span class="font-weight-bold">Leadership Solutions Academy</span> te ontsluiten heb je een code ontvangen.</p>
        </v-col>
        <v-col cols="12" class="horizontal-area horizontal-area_low">
          <p class="text-center">Geef deze code hieronder in om jouw persoonlijke programma te starten:</p>
        </v-col>
        <v-col cols="12" class="my-3 horizontal-area horizontal-area_low">
          <v-row justify="center" dense>
            <v-col cols="8">
              <input type="text" placeholder="Code">
            </v-col>
            <v-col cols="4" class="text-left bottom-list">
              <button class="button">Verstuur</button>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" class="horizontal-area horizontal-area_bottom">
          <p class="text-left">Je gaat straks door een spraakmakend programma op gebied van leiderschap. Wij houden je tussentijds op de hoogte van informatie die relevant is voor jouw leerervaring. Leadership Solutions gaat vertrouwelijk om met jouw informatie in lijn met onze
            <a href="#">privacy policy.</a></p>
        </v-col>
      </v-card-text>
    </v-card>
  </v-dialog>
</template>

<script>
export default {
  name: "GeefJeCodeDoor",
  data() {
    return {
      dialog: false
    }
  },
  props: {
    color: {
      default: 'white',
    },
  }
}
</script>

<style scoped>

.modal {
  padding-bottom: 100px;
  padding-top: 80px;
}

.horizontal-area {
  font-size: 50px;
}

.horizontal-area_low{
  font-family: Roboto;
  font-size: 25px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.6;
  letter-spacing: normal;
  text-align: center;
  color: #0d0303;
  width: 544px;
  margin: auto;
}

.horizontal-area_bottom{
  font-family: Roboto;
  font-size: 16px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.31;
  letter-spacing: normal;
  text-align: left;
  color: #0d0303;

  width: 663px;
  margin: auto;
}

input {
  border-radius: 8px;
  border: solid 2px #0d0303;
  font-family: Roboto;
  font-size: 20px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.3;
  letter-spacing: normal;
  text-align: left;
  color: #0d0303;
  padding-left: 19px;

  height: 70px;
}

input::placeholder {
  color: #a8a8a8;
}

.button {
  height: 70px;
  border-radius: 8px;
  border: solid 2px #0d0303;
  background-color: #0d0303;
  color: #ffffff;
  width: 100%;
}

</style>
