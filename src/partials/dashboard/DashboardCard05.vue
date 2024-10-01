<template>
  <div class="flex flex-col col-span-full sm:col-span-6 bg-white dark:bg-gray-800 shadow-sm rounded-xl">
    <header class="px-5 py-4 border-b border-gray-100 dark:border-gray-700/60 flex items-center">
      <h2 class="font-semibold text-gray-800 dark:text-gray-100">Sentiment Evolution</h2>
      <Tooltip class="ml-2">
        <div class="text-xs text-center whitespace-nowrap">Built with <a class="underline" href="https://www.chartjs.org/" target="_blank" rel="noreferrer">Chart.js</a></div>
      </Tooltip>
    </header>
    <!-- Chart built with Chart.js 3 -->
    <!-- Change the height attribute to adjust the chart height -->
    <RealtimeChart :data="chartData" width="595" height="248" />
  </div>
</template>

<script>
import { ref, computed, onMounted, onUnmounted, watch } from 'vue'
import Tooltip from '../../components/Tooltip.vue'
import { chartAreaGradient } from '../../charts/ChartjsConfig'
import RealtimeChart from '../../charts/RealtimeChart.vue'

// Import utilities
import { tailwindConfig, hexToRGB } from '../../utils/Utils'

export default {
  name: 'DashboardCard05',
  components: {
    Tooltip,
    RealtimeChart,
  },
  setup() {

    // IMPORTANT:
    // Code below is for demo purpose only, and it's not covered by support.
    // If you need to replace dummy data with real data,
    // refer to Chart.js documentation: https://www.chartjs.org/docs/latest    

    const counter = ref(0)
    const range = ref(35)

    // Dummy data to be looped
    const sampleData = [
      57.81, 55.75, 55.48, 54.28, 53.14, 52.25, 51.04, 52.49, 55.49, 56.87,
      53.73, 56.42, 58.06, 55.62, 58.16, 55.22, 58.67, 60.18, 61.31, 63.25,
      65.91, 64.44, 65.97, 62.27, 60.96, 59.34, 56.07, 59.85, 58.79, 61.92,
      60.95, 60.65, 59.09, 59.81, 61.85, 65.52, 62.21, 62.22, 64.42, 67.42,
      70.91, 68.52, 63.37, 67.58, 69.09, 69.36, 68.71, 67.42, 69.93, 68.71,
      67.62, 67.28, 65.37, 69.08, 67.94, 70.82, 72.94, 71.65, 72.25,
    ]
    
    const slicedData = ref(sampleData.slice(0, range.value))

    // Generate fake dates from now to back in time
    const generateDates = () => {
      const now = new Date()
      const dates = []
      sampleData.forEach((v, i) => {
        dates.push(new Date(now - 2000 - i * 2000))
      })
      return dates
    }
    
    const slicedLabels = ref(generateDates().slice(0, range.value).reverse())

    // Fake update every 2 seconds
    const interval = ref(null)
    onMounted(() => {
      interval.value = setInterval(() => {
        counter.value++
      }, 2000)
    })
    onUnmounted(() => {
      clearInterval(interval)
    })

    // Loop through data array and update
    watch(counter, () => {
      range.value++;
      if (range.value >= sampleData.length) {
        range.value = 0;
      }
      slicedData.value.shift();
      slicedData.value.push(sampleData[range.value]);      
      slicedLabels.value.shift()
      slicedLabels.value.push(new Date())
    })

    const chartData = computed(() => {
      return {
        labels: slicedLabels.value,
        datasets: [
          {
            data: [...slicedData.value],
            fill: true,
            backgroundColor: function(context) {
              const chart = context.chart;
              const {ctx, chartArea} = chart;
              return chartAreaGradient(ctx, chartArea, [
                { stop: 0, color: `rgba(${hexToRGB(tailwindConfig().theme.colors.violet[500])}, 0)` },
                { stop: 1, color: `rgba(${hexToRGB(tailwindConfig().theme.colors.violet[500])}, 0.2)` }
              ]);
            },
            borderColor: tailwindConfig().theme.colors.violet[500],
            borderWidth: 2,
            pointRadius: 0,
            pointHoverRadius: 3,
            pointBackgroundColor: tailwindConfig().theme.colors.violet[500],
            clip: 20,
            tension: 0.2,
          },
        ],
      }
    })

    return {
      counter,
      range,
      slicedData,
      slicedLabels,
      interval,
      chartData,
    }  
  }  
}
</script>