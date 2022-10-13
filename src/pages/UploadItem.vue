<template>
  <q-page class="flex flex-center">
    <q-card class="bg-secondary full-height"> 
  <div class="q-pa-md">
      <q-form>
          <q-input label="Im looking for.."> </q-input>
        <q-dialog transition-show="flip-down" transition-hide="flip-up" key="dialog-upload" v-model="dia"> 
              <q-uploader transition-show="flip-up" url="http://localhost:5000" key="files">test</q-uploader></q-dialog
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
<style>
    q-page {
        background: $purple-10;
    }
    </style>
