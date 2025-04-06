<script setup>
import Form from './components/Form.vue'
</script>

<template>
  <v-toolbar class="header" :elevation="8" title="RentImmo.renta"></v-toolbar>
  <Form></Form>
</template>

<style scoped>
.header {
  background-color: orange;
  color: white;
  margin-bottom: 3%;
}
</style>
