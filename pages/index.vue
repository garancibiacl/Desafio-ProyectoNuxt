<template>
  <v-container>
    <v-row>
      <v-col
        sm="12"
        md="6"
        lg="4"
        v-for="(personaje, index) in Characters"
        :key="index"
      >
        <Card :CharacterProp="personaje"></Card>
        <!--Se pasa prop padre al componente Card -->
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Characters from "../Characters"; // Se importa componente cards
export default {
  name: "IndexPage",

  data() {
    return {
      Characters: Characters,
    };
  },
};
</script>
 <style >
body {
  background: #255461 !important;
}
</style>