<script setup>
import { ref } from 'vue'

const firstName = ref('')

const rules = [
  (value) => {
    if (value) return true
    return 'You must enter a first name.'
  },
]
</script>

<template>
  <v-sheet class="mx-auto" width="300">
    <v-form @submit.prevent>
      <v-text-field v-model="firstName" :rules="rules" label="Prix d'achat"></v-text-field>
    </v-form>
    <v-form @submit.prevent>
      <v-text-field v-model="loyer" :rules="rules" label="Loyer mensuel"></v-text-field>
    </v-form>
    <v-form @submit.prevent>
      <v-text-field v-model="firstName" :rules="rules" label="Charges"></v-text-field>
    </v-form>
    <v-form @submit.prevent>
      <v-text-field v-model="firstName" :rules="rules" label="First name"></v-text-field>
      <v-btn class="mt-2" type="submit" block>Submit</v-btn>
    </v-form>
  </v-sheet>
</template>
