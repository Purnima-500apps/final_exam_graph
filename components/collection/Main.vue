<template>
   <div>
      <div class="text-center divide-y-2 border-y">
         <h1 class="text-3xl">Graph list</h1>
         <CollectionLine :LineChartData="LineChartData" />
       </div>

       <div class="text-center">
         <h1 class="text-3xl">Group Bar</h1>
         <CollectionBar />
       </div>
         
       <div class="text-center">
         <h1 class="text-3xl">Pie Bar</h1>
         <CollectionDonut :DonutChartData="DonutChartData"/>
       </div>
   </div>

</template>
<script setup lang="ts">


//Describing schema for GroupLine
interface LineSchema{
   title:object,
   subtitle:object,
   yAxis:object,
   xAxis:object,
   legend:object,
   plotOptions:object,
   series:object,
   responsive:object
}

interface  DonutSchema{
   chart:object,
   title:object,
   subtitle:object,
   plotOptions:object,
   series:object
}
 
let props = defineProps<{ LineChartData:LineSchema,DonutChartData:DonutSchema }>()

</script>