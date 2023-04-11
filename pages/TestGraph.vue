<template>
    <div>
        <h1>{{ "Bar Graph" }}</h1>
    <CollectionMain  type="chart" :BarChartData="BarChartData" />
    </div>
    
</template>

<script setup lang="ts">

import { BarChartData }  from '../ts/bar'

</script>

