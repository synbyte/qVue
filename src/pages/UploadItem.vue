<template>
  <q-page class="flex flex-center">
     <> 
  <div class="q-pa-md"><q-form><q-input label="Im looking for.."> </q-input></q-form></div>
  </q-page>
 

    </template>

<script>
import { defineComponent, ref, onMounted } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  setup(){
   return {
       dia:ref(true)
   }   
  },
  onMounted(){
      $q.fullscreen.request()
  }

})
</script>
