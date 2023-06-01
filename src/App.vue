<script setup>
import HeaderVue from './components/layouts/Header.vue'  
import FooterVue from './components/layouts/Footer.vue'
import { RouterLink, RouterView } from 'vue-router'

components:{
    HeaderVue, 
    FooterVue
}
</script>

<template>
    <Sidebar />
   <HeaderVue /> 
   <RouterView /> 
   <!-- <FooterVue /> -->
</template>










<style scoped>
 
</style>
