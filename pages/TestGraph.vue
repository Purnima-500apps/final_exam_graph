<template>
    
    <CollectionMain type="chart" :LineChartData="LineChartData" :DonutChartData="DonutChartData"/>

</template>

<script setup lang="ts">

import { LineChartData } from '../ts/line'
import { DonutChartData }  from '../ts/donut'

</script>