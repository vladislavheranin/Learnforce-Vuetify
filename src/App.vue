<template>
  <v-app>
    <app-header></app-header>

    <v-main>
      <v-container class="pa-0" fluid>
        <v-row dense>
          <v-col
              cols="12"
              class="card-container pa-0"
              color="white"
              height="960px"
          >
            <v-card class="rounded-0 pa-0 card-container__content">
              <v-img
                  :src="require('./assets/images/Angelien.jpg')"
                  class="white--text"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="960px"
              >
                <v-card-title style="margin-top: 7%;">
                  <v-row justify="center" dense class="mx-16">
                    <v-col cols="12" class="my-5 horizontal-area horizontal-area_low">
                      <p class="font-weight-black white--text text-center">Hi Marcel </p>
                    </v-col>
                    <v-col cols="12" class="my-5 horizontal-area horizontal-area_low">
                      <p class="font-weight-black white--text text-center">Welkom bij Leadership Solutions!</p>
                    </v-col>

                    <v-col cols="12" class="my-5 pa-4 horizontal-area horizontal-area_low__light">
                      <p class=" white--text text-center">Het platform waar jij kunt ontdekken hoe je succesvol kunt zijn op het gebied van leiderschap.</p>
                    </v-col>

                    <v-col cols="12" class="my-14 text-center horizontal-area">
                      <div class="text-center">
                        <geef-je-code-door></geef-je-code-door>
                      </div>
                    </v-col>

                    <v-col cols="3">
                      <v-row justify="center" dense>
                        <v-col cols="1">
                          <v-icon
                            color="white"
                            size="24px"
                          >
                            mdi-checkbox-marked-circle-outline
                          </v-icon>
                        </v-col>
                        <v-col cols="8" class="text-left bottom-list">24 lessen over persoonlijk leiderschap</v-col>
                      </v-row>
                    </v-col>
                    <v-col cols="3">
                      <v-row justify="center" dense>
                        <v-col cols="1">
                          <v-icon
                              color="white"
                              size="24px"
                          >
                            mdi-checkbox-marked-circle-outline
                          </v-icon>
                        </v-col>
                        <v-col cols="8" class="text-left bottom-list">Ga verder waar je gebleven bent. </v-col>
                      </v-row>
                    </v-col>
                    <v-col cols="3">
                      <v-row justify="center" dense>
                        <v-col cols="1">
                          <v-icon
                              color="white"
                              size="24px"
                          >
                            mdi-checkbox-marked-circle-outline
                          </v-icon>
                        </v-col>
                        <v-col cols="8" class="text-left bottom-list">Spraakmakende webinars en live events</v-col>
                      </v-row>
                    </v-col>
                    <v-col cols="3">
                      <v-row justify="center" dense>
                        <v-col cols="1">
                          <v-icon
                              color="white"
                              size="24px"
                          >
                            mdi-checkbox-marked-circle-outline
                          </v-icon>
                        </v-col>
                        <v-col cols="8" class="text-left bottom-list">Inclusief werkboeken om verder te verdiepeIn</v-col>
                      </v-row>
                    </v-col>
                  </v-row>
                </v-card-title>
              </v-img>
            </v-card>
          </v-col>
          <content-half-item
          title="Wat leuk dat we deze reis samen aan gaan"
          sub-title="Zoek je de juiste handvatten om echt door te zetten? Ben jij klaar voor de volgende stap in je carrière? Ik geloof in jouw succes! Samen gaan we aan de slag met ingrediënten voor persoonlijke groei."
          type="signature"
          ></content-half-item>
          <photo-half-item img-link="assets/images/Angelien.jpg"></photo-half-item>

          <photo-half-item img-link="https://cdn.vuetifyjs.com/images/cards/plane.jpg"></photo-half-item>
          <content-half-item-green
              title="Ieder deel van de training heeft een werkboek"
              sub-title="Zo verdiep je de materie en krijg je praktische opdrachten om het geleerde meteen in de praktijk te brengen."
              type="btn"
          ></content-half-item-green>

          <content-half-item
              title="Spraakmakende webinars & events"
              sub-title="In het programma wordt je geregeld uitgenodigd voor webinars, ask-me-anything calls en live events. Heb je gerichte vragen of uitdagingen? Stel ze in de webinars en je krijgt persoonlijk advies."
          ></content-half-item>
          <photo-half-item img-link="https://cdn.vuetifyjs.com/images/cards/plane.jpg"></photo-half-item>

          <photo-half-item img-link="https://cdn.vuetifyjs.com/images/cards/plane.jpg"></photo-half-item>
          <content-half-item-green
              title="Leer met iedere device, waar je ook bent op eigen tempo"
              sub-title="Wisselen van laptop naar tablet of mobiel? Geen enkel probleem! Log in met je andere device en je kunt meteen verder waar je gebleven was. Wel zo handig."
              class="text-bg"
          ></content-half-item-green>
          <v-col cols="12" class="pa-16 horizontal-subtitle">
            <p class="font-weight-black black--text text-center">Over de trainers</p>
          </v-col>
          <v-col lg="3" xl="3" cols="0" md="0" sm="0" xs="0" class="pa-0"></v-col>
          <v-col cols="12" lg="3" xl="3" md="12" sm="12" class="pa-0">
            <v-card elevation="0" class="rounded-0">
              <v-img
                  :src="require('./assets/images/module00.jpg')"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="700px"
              >
              </v-img>
            </v-card>
          </v-col>
          <v-col cols="12" lg="3" xl="3" md="12" sm="12" class="pa-0">
            <v-card elevation="0" class="rounded-0">
              <v-img
                  :src="require('./assets/images/module00.jpg')"
                  class="white--text align-end"
                  gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
                  height="700px"
              >
              </v-img>
            </v-card>
          </v-col>
          <v-col cols="12" class="mt-8 horizontal-area horizontal-area__big">
            <p class="font-weight-black black--text text-center">11:04:06</p>
          </v-col>
          <v-col cols="12" class="my-5 horizontal-area">
            <p class="font-weight-black black--text text-center">Your journey starts now </p>
          </v-col>
          <v-col cols="12" class="my-14 text-center horizontal-area">
            <geef-je-code-door color="#070000"></geef-je-code-door>
          </v-col>
        </v-row>
      </v-container>
    </v-main>

    <app-footer></app-footer>
  </v-app>
</template>

<script>
import AppFooter from "@/components/base/AppFooter";
import AppHeader from "@/components/base/AppHeader";

import PhotoHalfItem from "@/components/halfItem/PhotoHalfItem";
import ContentHalfItem from "@/components/halfItem/ContentHalfItem";
import ContentHalfItemGreen from "@/components/halfItem/ContentHalfItemGreen";

import GeefJeCodeDoor from "@/components/modals/GeefJeCodeDoor";

export default {
  name: 'App',
  data: () => ({
    cards: [
      { title: 'Pre-fab homes', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 12 },
    ],
    items: [
      {title: 'Pre-fab homes', subTitle: 'Pre-fab homes', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', type: null, _id: 'item_0'}
    ],
  }),
  components: {
    AppFooter,
    AppHeader,
    PhotoHalfItem,
    ContentHalfItem,
    ContentHalfItemGreen,
    GeefJeCodeDoor
}
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}


.horizontal-area{
  font-family: Neuton;
  font-size: 70px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.27;
  letter-spacing: normal;
  text-align: left;
  color: #011014;
}
.horizontal-subtitle {
  font-size: 30px;
}
.horizontal-area__big{
  font-size: 90px;
}
.horizontal-area_low{
  font-size: 60px;
}
.horizontal-area_low__light {
  font-family: Roboto;
  font-size: 30px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.67;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
}
.horizontal-subtitle {
  background-color: #fcfafa;
}
.card-container {
  font-size: 2.5em;
}
.card-container__content {
  padding-left: 150px;
  padding-right: 150px;
  padding-top: 150px;

  font-family: Roboto;
  font-size: 35px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.57;
  letter-spacing: normal;
  text-align: left;
  color: #091f24;
}

.bottom-list {
  word-break: break-word;
}
*:focus {
  outline: none;
}

@media (max-width: 1400px) {
  .card-container, h3, h4 {
    font-size: 0.8em !important;
  }
  .card-container__content {
    padding-left: 80px;
    padding-right: 80px;
    padding-top: 80px;
  }
  .horizontal-area__big{
    font-size: 50px;
  }
  .horizontal-area_low{
    font-size: 30px;
  }
  .horizontal-subtitle {
    font-size: 50px;
  }
}
@media (min-width: 1400px) {
  .card-container__content {
    padding-left: 100px;
    padding-right: 100px;
    padding-top: 100px;
  }
  .horizontal-area_low__light {
    flex: 0 0 50% !important;
    max-width: 50% !important;
  }
  .horizontal-subtitle {
    font-size: 70px;
  }
}

@media (max-width: 1024px) {
  .card-container, h3, h4 {
    font-size: 0.8em !important;
  }
  .horizontal-area__big{
    font-size: 50px;
  }
  .horizontal-area_low{
    font-size: 30px;
  }
}

@media (max-width: 600px) {
  .card-container__content {
    padding-left: 25px;
    padding-right: 25px;
    padding-top: 25px;
  }
  .horizontal-subtitle {
    font-size: 30px;
  }
}
</style>
