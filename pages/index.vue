<template>
  <div class="container">
   <Hero />
   <LargeCardDisplay 
    v-for="cardInfo in largeCardInfo" :key="cardInfo.id" :cardSection="cardInfo"/>
  </div>
</template>

<script>
//@root
import {largeCardSections} from "@/assets/data.js"
export default {
  data(){
    return{
      largeCardInfo: largeCardSections
    }
  }
}
</script>

<style>

</style>
