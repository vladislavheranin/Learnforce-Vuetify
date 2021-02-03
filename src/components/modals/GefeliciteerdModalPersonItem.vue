<template>
    <v-card
        width="360"
        height="100"
        tile
    >
      <v-row no-gutters>
        <v-col cols="3" class="pa-0 ma-0">
          <v-avatar
              width="100"
              height="100"
              tile
          >
            <v-img src="https://cdn.vuetifyjs.com/images/cards/plane.jpg"></v-img>
          </v-avatar>
        </v-col>
        <v-col class="pa-0 ma-0" cols="8">
          <div class="text-block">
            Find your leadership style in 3 steps
          </div>
        </v-col>
      </v-row>
    </v-card>
</template>

<script>
export default {
  name: "GefeliciteerdModalPersonItem"
}
</script>

<style scoped>

.text-block {
  width: 100%;
  padding-top: 22px;
  padding-left: 35px;
  font-family: Roboto;
  font-size: 20px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.25;
  letter-spacing: normal;
  text-align: left;
  color: #091f24;
}

</style>
