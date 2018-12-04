<template>
  <v-card class="dog-card">
    <v-img height="150px" :src="dog"></v-img>
    <v-card-actions>
      <v-spacer></v-spacer>
      <v-btn icon @click="$emit('remove');"> <v-icon>delete</v-icon> </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  props: {
    dog: {
      type: String
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!-- con scoped se queda el estilo acoplado al componente -->
<style scoped></style>
