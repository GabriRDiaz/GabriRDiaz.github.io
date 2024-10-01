<template>
  <div class="col-span-full xl:col-span-6 bg-white dark:bg-gray-800 shadow-sm rounded-xl">
    <header class="px-5 py-4 border-b border-gray-100 dark:border-gray-700/60">
      <h2 class="font-semibold text-gray-800 dark:text-gray-100">Recent Reviews</h2>
    </header>
    <div class="p-3">

      <!-- Card content -->
      <!-- "Today" group -->
      <div>
        <header class="text-xs uppercase text-gray-400 dark:text-gray-500 bg-gray-50 dark:bg-gray-700 dark:bg-opacity-50 rounded-sm font-semibold p-2">Today</header>
        <ul class="my-1">
          <!-- Item -->
          <li class="flex px-2">
            <div class="w-9 h-9 rounded-full shrink-0 bg-green-500 my-2 mr-3">
              <svg class="w-9 h-9 fill-current text-white" viewBox="0 0 36 36">
                <path d="M18 10c-4.4 0-8 3.1-8 7s3.6 7 8 7h.6l5.4 2v-4.4c1.2-1.2 2-2.8 2-4.6 0-3.9-3.6-7-8-7zm4 10.8v2.3L18.9 22H18c-3.3 0-6-2.2-6-5s2.7-5 6-5 6 2.2 6 5c0 2.2-2 3.8-2 3.8z" />
              </svg>
            </div>
            <div class="grow flex items-center border-b border-gray-100 dark:border-gray-700/60 text-sm py-2">
              <div class="grow flex justify-between">
                <div class="self-center"><a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">User89379127</a> left a review with <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">5 stars</a>, the main topic was <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">service</a></div>
                <div class="shrink-0 self-end ml-2">
                  <a class="font-medium text-violet-500 hover:text-violet-600 dark:hover:text-violet-400" href="#0">View<span class="hidden sm:inline"> -&gt;</span></a>
                </div>
              </div>
            </div>
          </li>
          <!-- Item -->
          <li class="flex px-2">
            <div class="w-9 h-9 rounded-full shrink-0 bg-red-500 my-2 mr-3">
              <svg class="w-9 h-9 fill-current text-white" viewBox="0 0 36 36">
                <path d="M18 10c-4.4 0-8 3.1-8 7s3.6 7 8 7h.6l5.4 2v-4.4c1.2-1.2 2-2.8 2-4.6 0-3.9-3.6-7-8-7zm4 10.8v2.3L18.9 22H18c-3.3 0-6-2.2-6-5s2.7-5 6-5 6 2.2 6 5c0 2.2-2 3.8-2 3.8z" />
              </svg>
            </div>
            <div class="grow flex items-center border-b border-gray-100 dark:border-gray-700/60 text-sm py-2">
              <div class="grow flex justify-between">
                <div class="self-center"><a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">User72387162</a> left a review with <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">2 stars</a>, the main topic was <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">toilets</a></div>
                <div class="shrink-0 self-end ml-2">
                  <a class="font-medium text-violet-500 hover:text-violet-600 dark:hover:text-violet-400" href="#0">View<span class="hidden sm:inline"> -&gt;</span></a>
                </div>
              </div>
            </div>
          </li>
          <!-- Item -->
          <li class="flex px-2">
            <div class="w-9 h-9 rounded-full shrink-0 bg-green-500 my-2 mr-3">
              <svg class="w-9 h-9 fill-current text-white" viewBox="0 0 36 36">
                <path d="M18 10c-4.4 0-8 3.1-8 7s3.6 7 8 7h.6l5.4 2v-4.4c1.2-1.2 2-2.8 2-4.6 0-3.9-3.6-7-8-7zm4 10.8v2.3L18.9 22H18c-3.3 0-6-2.2-6-5s2.7-5 6-5 6 2.2 6 5c0 2.2-2 3.8-2 3.8z" />
              </svg>
            </div>
            <div class="grow flex items-center text-sm py-2">
              <div class="grow flex justify-between">
                <div class="self-center"><a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">User382739</a> left a review with <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">4 stars</a>, the main topic was <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">food</a></div>
                <div class="shrink-0 self-end ml-2">
                  <a class="font-medium text-violet-500 hover:text-violet-600 dark:hover:text-violet-400" href="#0">View<span class="hidden sm:inline"> -&gt;</span></a>
                </div>
              </div>
            </div>
          </li>
        </ul>
      </div>
      <!-- "Yesterday" group -->
      <div>
        <header class="text-xs uppercase text-gray-400 dark:text-gray-500 bg-gray-50 dark:bg-gray-700 dark:bg-opacity-50 rounded-sm font-semibold p-2">Yesterday</header>
        <ul class="my-1">
          <!-- Item -->
          <li class="flex px-2">
            <div class="w-9 h-9 rounded-full shrink-0 bg-green-500 my-2 mr-3">
              <svg class="w-9 h-9 fill-current text-white" viewBox="0 0 36 36">
                <path d="M18 10c-4.4 0-8 3.1-8 7s3.6 7 8 7h.6l5.4 2v-4.4c1.2-1.2 2-2.8 2-4.6 0-3.9-3.6-7-8-7zm4 10.8v2.3L18.9 22H18c-3.3 0-6-2.2-6-5s2.7-5 6-5 6 2.2 6 5c0 2.2-2 3.8-2 3.8z" />
              </svg>
            </div>
            <div class="grow flex items-center border-b border-gray-100 dark:border-gray-700/60 text-sm py-2">
              <div class="grow flex justify-between">
                <div class="self-center"><a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">User89379127</a> left a review with <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">5 stars</a>, the main topic was <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">service</a></div>
                <div class="shrink-0 self-end ml-2">
                  <a class="font-medium text-violet-500 hover:text-violet-600 dark:hover:text-violet-400" href="#0">View<span class="hidden sm:inline"> -&gt;</span></a>
                </div>
              </div>
            </div>
          </li>
          <!-- Item -->
          <li class="flex px-2">
            <div class="w-9 h-9 rounded-full shrink-0 bg-blue-100 my-2 mr-3">
              <svg class="w-9 h-9 fill-current text-white" viewBox="0 0 36 36">
                <path d="M18 10c-4.4 0-8 3.1-8 7s3.6 7 8 7h.6l5.4 2v-4.4c1.2-1.2 2-2.8 2-4.6 0-3.9-3.6-7-8-7zm4 10.8v2.3L18.9 22H18c-3.3 0-6-2.2-6-5s2.7-5 6-5 6 2.2 6 5c0 2.2-2 3.8-2 3.8z" />
              </svg>
            </div>
            <div class="grow flex items-center border-b border-gray-100 dark:border-gray-700/60 text-sm py-2">
              <div class="grow flex justify-between">
                <div class="self-center"><a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">User72387162</a> left a review with <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">3 stars</a>, the main topic was <a class="font-medium text-gray-800 hover:text-gray-900 dark:text-gray-100 dark:hover:text-white" href="#0">toilets</a></div>
                <div class="shrink-0 self-end ml-2">
                  <a class="font-medium text-violet-500 hover:text-violet-600 dark:hover:text-violet-400" href="#0">View<span class="hidden sm:inline"> -&gt;</span></a>
                </div>
              </div>
            </div>
          </li>
        </ul>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'DashboardCard12',
}
</script>