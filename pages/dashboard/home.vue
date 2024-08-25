<script setup >


// import { createPinia } from 'pinia'
// import { createApp } from 'vue'


// const pinia = createPinia()
// const app = createApp(home)
// app.use(pinia)


import {useAlertStore} from '@/stores/alertstore';


const store = useAlertStore();



console.log(store)





</script>




<template>
  <div>
    <h1 class="text-8xl text-center mt-8">Home</h1>
    <button
      @click="store.alert"
      class="h-12 w-24 ml-96 rounded-lg text-2xl bg-red-500 text-white"
    >
      click
    </button>
  </div>
</template>


