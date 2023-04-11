<template>

   <vue-highCharts type="chart" :options="chartData" />

</template>

<script setup lang="ts">

import VueHighCharts from 'vue3-highcharts';

interface  DonutSchema{
  chart:object,
  title:object,
  subtitle:object,
  plotOptions:object,
  series:object
}

let props = defineProps<{ DonutChartData:DonutSchema }>()

const chartData = computed(() => {
  return props.DonutChartData
})
</script>