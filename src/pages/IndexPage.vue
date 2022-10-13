<template>
  <q-page class="flex flex-center">
 <q-btn to="/upload"><q-icon name="upload"></q-icon>Upload Photos</q-btn>
 <span></span>
   
  </q-page>
  <!--<q-dialog v-model="dia">     
              <q-uploader  url='http://localhost:4444/upload'></q-uploader>
</q-dialog>        -->      
  
 
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
      $q.fullscreen.request();
      $q.dark.set(true);
  }

})
</script>
