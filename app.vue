<template>
  <div> 
   <Admin >
    <NuxtPage />
    </Admin>
  </div>
</template>

<script>
import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'
//import Admin from './layouts/Admin'

export default {
 components:{
    //Admin,
 }
};

onMounted(() => {
    initFlowbite();
})

</script>

<style>

</style>
