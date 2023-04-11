<template>
   <div>
      <div class="text-center divide-y-2 border-y">
         <h1 class="text-3xl">Graph list</h1>
       </div>

       <div class="text-center">
         <h1 class="text-3xl">Group Bar</h1>
         <CollectionBar :BarChartData="BarChartData"/>
       </div>
         
       
   </div>

</template>
<script setup lang="ts">

interface BarSchema{
   chart:object,
   title:object,
   xAxis:object,
   yAxis:object,
   tooltip:object,
   plotOptions:object,
   series:object
}
 
let props = defineProps<{ BarChartData:BarSchema}>()

</script>