<template>
   <div>
      <vue-highCharts type="chart" :options="chartData" />
   </div>
</template>
<script setup lang="ts">

import VueHighCharts from 'vue3-highcharts'

interface BarSchema{
   chart:object,
   title:object,
   xAxis:object,
   yAxis:object,
   tooltip:object,
   plotOptions:object,
   series:object

}

let props = defineProps<{ BarChartData:BarSchema }>()

const chartData = computed(() => {
   return props.BarChartData
})
</script>