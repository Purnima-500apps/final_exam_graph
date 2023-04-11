<template>
    <vue-highCharts type="chart" :options="chartData" />
</template>

<script setup lang="ts">
import VueHighCharts from 'vue3-highcharts';
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

let props = defineProps<{ LineChartData:LineSchema }>()

const chartData = computed(() => {
   return props.LineChartData
})
</script>