<template>
  <q-page class="flex flex-center">
    <q-card class="full-height"> 
  <div class="q-pa-md"><q-form><q-input label="Im looking for.."> </q-input><q-dialog v-model="dia"><q-upload url="http://localhost:5000">test</q-upload></q-dialog
  ><q-btn @click="dia = true"><q-icon name="upload"></q-icon>Upload Photos</q-btn></q-form></div></q-card>
  </q-page>
 

    </template>

<script>
import { defineComponent, ref, onMounted } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  setup(){
   return {
       dia:ref(false)
   }   
  },
  onMounted(){
      $q.fullscreen.request()
  }

})
</script>
