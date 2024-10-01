<template>
  <div class="flex flex-col col-span-full sm:col-span-6 xl:col-span-4 bg-white dark:bg-gray-800 shadow-sm rounded-xl">
    <header class="px-5 py-4 border-b border-gray-100 dark:border-gray-700/60">
      <h2 class="font-semibold text-gray-800 dark:text-gray-100">Sentiment Analysis</h2>
    </header>
    <!-- Chart built with Chart.js 3 -->
    <!-- Change the height attribute to adjust the chart height -->
    <DoughnutChart :data="chartData" width="389" height="260" />
  </div>
</template>

<script>
import { ref } from 'vue'
import DoughnutChart from '../../charts/DoughnutChart.vue'

// Import utilities
import { tailwindConfig } from '../../utils/Utils'

export default {
  name: 'DashboardCard06',
  components: {
    DoughnutChart,
  },
  setup() {
    const chartData = ref({
      labels: ['Positive', 'Neutral', 'Negative'],
      datasets: [
        {
          label: 'Number of reviews',
          data: [
            60, 25, 15,
          ],
          backgroundColor: [
            tailwindConfig().theme.colors.green[500],
            tailwindConfig().theme.colors.gray[50],
            tailwindConfig().theme.colors.red[50],
          ],
          hoverBackgroundColor: [
            tailwindConfig().theme.colors.green[600],
            tailwindConfig().theme.colors.gray[600],
            tailwindConfig().theme.colors.red[900],
          ],
          borderWidth: 0,
        },
      ],
    })

    return {
      chartData,
    } 
  }
}
</script>