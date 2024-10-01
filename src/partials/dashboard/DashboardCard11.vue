<template>
  <div class="flex flex-col col-span-full sm:col-span-6 bg-white dark:bg-gray-800 shadow-sm rounded-xl">
    <header class="px-5 py-4 border-b border-gray-100 dark:border-gray-700/60 flex items-center">
      <h2 class="font-semibold text-gray-800 dark:text-gray-100">Main Topics</h2>
    </header>
    <div class="px-5 py-3">
      <div class="flex items-start">
        <div class="text-3xl font-bold text-gray-800 dark:text-gray-100 mr-2">Service</div>
      </div>
    </div>    
    <!-- Chart built with Chart.js 3 -->
    <div class="grow">
      <!-- Change the height attribute to adjust the chart height -->
      <BarChart :data="chartData" :width="595" :height="48" />
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'
import BarChart from '../../charts/BarChart03.vue'

// Import utilities
import { tailwindConfig } from '../../utils/Utils'

export default {
  name: 'DashboardCard11',
  components: {
    BarChart,
  },  
  setup() {
    const chartData = ref({
      labels: ['Reasons'],
      datasets: [
        {
          label: 'Service',
          data: [37],
          backgroundColor: tailwindConfig().theme.colors.violet[500],
          hoverBackgroundColor: tailwindConfig().theme.colors.violet[600],
          barPercentage: 1,
          categoryPercentage: 1,
        },
        {
          label: 'Food',
          data: [23],
          backgroundColor: tailwindConfig().theme.colors.violet[700],
          hoverBackgroundColor: tailwindConfig().theme.colors.violet[800],
          barPercentage: 1,
          categoryPercentage: 1,
        },
        {
          label: 'Prices',
          data: [18],
          backgroundColor: tailwindConfig().theme.colors['sky'][500],
          hoverBackgroundColor: tailwindConfig().theme.colors['sky'][600],
          barPercentage: 1,
          categoryPercentage: 1,
        },
        {
          label: 'Location',
          data: [12],
          backgroundColor: tailwindConfig().theme.colors.green[500],
          hoverBackgroundColor: tailwindConfig().theme.colors.green[600],
          barPercentage: 1,
          categoryPercentage: 1,
        },
        {
          label: 'Others',
          data: [10],
          backgroundColor: tailwindConfig().theme.colors.gray[200],
          hoverBackgroundColor: tailwindConfig().theme.colors.gray[300],
          barPercentage: 1,
          categoryPercentage: 1,
        },
      ],
    })

    return {
      chartData,
    } 
  }
}
</script>