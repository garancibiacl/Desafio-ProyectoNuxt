<template>
  <div class="pa-10">
    <v-card class="bg-title" max-width="344">
      <v-img :src="CharacterProp.imagen" height="200px"></v-img>

      <v-card-title class="d-flex justify-space-between">{{ CharacterProp.nombre }}
<div>
            <v-btn icon style="color: #00DC82;">
                <v-icon>mdi-heart</v-icon>
              </v-btn>

              <v-btn icon style="color: #00DC82;" >
                <v-icon class="">mdi-bookmark</v-icon>
              </v-btn>

              <v-btn icon style="color: #00DC82;">
                <v-icon>mdi-share-variant</v-icon>
              </v-btn>
              </div>
      </v-card-title>
    </v-card>
  </div>
</template>
<script>
export default {
  props: ["CharacterProp"],
  data() {},
};
</script>

<style scoped>
.v-card {
  margin: auto; 
}
.bg-title{
        background: #003543;
}
.icon-color{
    color: #00DC82;
}
</style>