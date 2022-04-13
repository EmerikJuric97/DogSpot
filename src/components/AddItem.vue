<template>
  <v-dialog persistent :value="value" width="500">
    <v-card>
      <v-card-title>Add Item</v-card-title>
      <v-card-text>Lorem ipsum</v-card-text>
      <v-card-actions>
        <v-spacer/>
        <v-btn text @click="$emit('input', false)">Close Dialog</v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
</template>
<script>
export default {
  name: "add-item",
  props: ["value"]
};
</script>