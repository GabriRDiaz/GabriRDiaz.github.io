<template>
  <div class="col-span-full xl:col-span-8 bg-white dark:bg-gray-800 shadow-sm rounded-xl">
    <header class="px-5 py-4 border-b border-gray-100 dark:border-gray-700/60">
      <h2 class="font-semibold text-gray-800 dark:text-gray-100">Top Channels</h2>
    </header>
    <div class="p-3">

      <!-- Table -->
      <div class="overflow-x-auto">
        <table class="table-auto w-full dark:text-gray-300">
          <!-- Table header -->
          <thead class="text-xs uppercase text-gray-400 dark:text-gray-500 bg-gray-50 dark:bg-gray-700 dark:bg-opacity-50 rounded-sm">
            <tr>
              <th class="p-2">
                <div class="font-semibold text-left">Source</div>
              </th>
              <th class="p-2">
                <div class="font-semibold text-center">Reviews</div>
              </th>
              <th class="p-2">
                <div class="font-semibold text-center">Increase</div>
              </th>
              <th class="p-2">
                <div class="font-semibold text-center">Sales</div>
              </th>
              <th class="p-2">
                <div class="font-semibold text-center">Conversion</div>
              </th>
            </tr>
          </thead>
          <!-- Table body -->
          <tbody class="text-sm font-medium divide-y divide-gray-100 dark:divide-gray-700/60">
            <!-- Row -->
            <tr>
              <td class="p-2">
                <div class="flex items-center">
                  <svg class="shrink-0 mr-2 sm:mr-3" width="36" height="36" viewBox="0 0 36 36">
                    <circle fill="#1DA1F2" cx="18" cy="18" r="18" />
                    <g transform="scale(0.7) translate(10,10)"><path d="M32.001 7.075a12.94 12.94 0 0 1-3.771 1.034 6.588 6.588 0 0 0 2.887-3.632 13.043 13.043 0 0 1-4.152 1.581 6.563 6.563 0 0 0-4.797-2.078c-3.63 0-6.573 2.944-6.573 6.574 0 .515.057 1.016.17 1.496-5.465-.274-10.308-2.889-13.551-6.863a6.535 6.535 0 0 0-.89 3.304 6.571 6.571 0 0 0 2.922 5.471 6.527 6.527 0 0 1-2.978-.823v.083c0 3.17 2.255 5.814 5.25 6.416a6.56 6.56 0 0 1-2.968.113c.837 2.613 3.263 4.514 6.138 4.567a13.163 13.163 0 0 1-8.14 2.807c-.53 0-1.05-.031-1.565-.091a18.558 18.558 0 0 0 10.045 2.944c12.054 0 18.646-9.99 18.646-18.646 0-.284-.007-.568-.02-.85A13.3 13.3 0 0 0 32.001 7.075z"
                      fill="white" /></g>
                  </svg>
                  <div class="text-gray-800 dark:text-gray-100">X.com</div>
                </div>
              </td>
              <td class="p-2">
                <div class="text-center">2.4K</div>
              </td>
              <td class="p-2">
                <div class="text-center text-green-500">877</div>
              </td>
              <td class="p-2">
                <div class="text-center">267</div>
              </td>
              <td class="p-2">
                <div class="text-center text-sky-500">4.7</div>
              </td>
            </tr>
            <!-- Row -->
            <tr>
              <td class="p-2">
                <div class="flex items-center">
                  <svg class="shrink-0 mr-2 sm:mr-3" width="36" height="36" viewBox="0 0 36 36">
                    <circle fill="#1877F2" cx="18" cy="18" r="18" />
                    <path d="M16.023 26 16 19h-3v-3h3v-2c0-2.7 1.672-4 4.08-4 1.153 0 2.144.086 2.433.124v2.821h-1.67c-1.31 0-1.563.623-1.563 1.536V16H23l-1 3h-2.72v7h-3.257Z" fill="#FFF" fill-rule="nonzero" />
                  </svg>
                  <div class="text-gray-800 dark:text-gray-100">Facebook</div>
                </div>
              </td>
              <td class="p-2">
                <div class="text-center">2.2K</div>
              </td>
              <td class="p-2">
                <div class="text-center text-green-500">287</div>
              </td>
              <td class="p-2">
                <div class="text-center">249</div>
              </td>
              <td class="p-2">
                <div class="text-center text-sky-500">4.4</div>
              </td>
            </tr>
            <!-- Row -->
            <tr>
              <td class="p-2">
                <div class="flex items-center">
                  <svg class="shrink-0 mr-2 sm:mr-3" width="36" height="36" viewBox="0 0 36 36">
                    <circle fill="#EA4335" cx="18" cy="18" r="18" />
                    <path d="M18 17v2.4h4.1c-.2 1-1.2 3-4 3-2.4 0-4.3-2-4.3-4.4 0-2.4 2-4.4 4.3-4.4 1.4 0 2.3.6 2.8 1.1l1.9-1.8C21.6 11.7 20 11 18.1 11c-3.9 0-7 3.1-7 7s3.1 7 7 7c4 0 6.7-2.8 6.7-6.8 0-.5 0-.8-.1-1.2H18z" fill="#FFF" fill-rule="nonzero" />
                  </svg>
                  <div class="text-gray-800 dark:text-gray-100">Google (organic)</div>
                </div>
              </td>
              <td class="p-2">
                <div class="text-center">2.0K</div>
              </td>
              <td class="p-2">
                <div class="text-center text-green-500">434</div>
              </td>
              <td class="p-2">
                <div class="text-center">224</div>
              </td>
              <td class="p-2">
                <div class="text-center text-sky-500">4.2</div>
              </td>
            </tr>
            <!-- Row -->
            <tr>
              <td class="p-2">
                <div class="flex items-center">
                  <svg class="shrink-0 mr-2 sm:mr-3" width="36" height="36" viewBox="0 0 512 512" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="256" cy="256" r="256" fill="#E4405F"/>
                      <!-- Outer camera shape -->
                      <path d="M373.7 124H138.3c-36.5 0-66.3 29.8-66.3 66.3v166.4c0 36.5 29.8 66.3 66.3 66.3h235.4c36.5 0 66.3-29.8 66.3-66.3V204.3c0-36.5-29.8-66.3-66.3-66.3zM256 346.7c-50.1 0-90.7-40.6-90.7-90.7s40.6-90.7 90.7-90.7 90.7 40.6 90.7 90.7-40.6 90.7-90.7 90.7zm109.2-157.6c-13.6 0-24.6-11-24.6-24.6s11-24.6 24.6-24.6 24.6 11 24.6 24.6-11 24.6-24.6 24.6z" fill="#FFF"/>

                      <!-- Camera lens circle -->
                      <circle cx="256" cy="256" r="60" fill="#FFF"/>
                  </svg>                                  
                  <div class="text-gray-800 dark:text-gray-100">Instagram.com</div>
                </div>
              </td>
              <td class="p-2">
                <div class="text-center">1.9K</div>
              </td>
              <td class="p-2">
                <div class="text-center text-green-500">203</div>
              </td>
              <td class="p-2">
                <div class="text-center">220</div>
              </td>
              <td class="p-2">
                <div class="text-center text-sky-500">4.2</div>
              </td>
            </tr>
            <tr>
              <td class="p-2">
                <div class="flex items-center">
                  <svg class="shrink-0 mr-2 sm:mr-3" width="36" height="36" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
      <!-- Outer circle representing the globe -->
      <circle cx="32" cy="32" r="30" fill="#007BFF" />
      <!-- Horizontal and vertical lines -->
      <path d="M2 32h60M32 2v60" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" />
      <!-- Curved lines to represent latitude -->
      <path d="M32 10a22 22 0 0 1 0 44" stroke="#FFFFFF" stroke-width="2" fill="none" />
      <path d="M32 18a14 14 0 0 1 0 28" stroke="#FFFFFF" stroke-width="2" fill="none" />
      <path d="M32 22a10 10 0 0 1 0 20" stroke="#FFFFFF" stroke-width="2" fill="none" />
      <!-- Nodes for network representation -->
      <circle cx="32" cy="10" r="2" fill="#FFFFFF" />
      <circle cx="32" cy="54" r="2" fill="#FFFFFF" />
      <circle cx="10" cy="32" r="2" fill="#FFFFFF" />
      <circle cx="54" cy="32" r="2" fill="#FFFFFF" />
      <circle cx="20" cy="20" r="2" fill="#FFFFFF" />
      <circle cx="44" cy="20" r="2" fill="#FFFFFF" />
      <circle cx="20" cy="44" r="2" fill="#FFFFFF" />
      <circle cx="44" cy="44" r="2" fill="#FFFFFF" />
    </svg>
                  <div class="text-gray-800 dark:text-gray-100">Webpage</div>
                </div>
              </td>
              <td class="p-2">
                <div class="text-center">2.2K</div>
              </td>
              <td class="p-2">
                <div class="text-center text-green-500">287</div>
              </td>
              <td class="p-2">
                <div class="text-center">249</div>
              </td>
              <td class="p-2">
                <div class="text-center text-sky-500">4.4</div>
              </td>
            </tr>
          </tbody>
        </table>

      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DashboardCard07',
}
</script>