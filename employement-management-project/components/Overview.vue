<template>
  <div class="col-span-1 lg:col-span-2 bg-white p-2 shadow">
    <div class="mx-3 my-2 flex items-center justify-between">
      <h2 class="text-2xl pb-2 font-semibold">Good Morning, Turja Sen</h2>
      <p class="text-sm font-semibold text-gray-500">03 Jan - 31 Jan 2025</p>
      <div class="w-30 h-10 flex items-center justify-between  bg-purple-700 text-white px-5 py-2 rounded hover:bg-purple-500">
        <DownloadIcon class="w-5 h-5" />
        <button
          class=""
        >
          Export Data
        </button>
      </div>
    </div>
    <div class=" mx-3 grid grid-cols-1 md:grid-cols-3 gap-4">
      <EmployeesCount />
      <AttendanceOverView />
      <DevicesUsed />
    </div>
  </div>
</template>

<script setup>
import { DownloadIcon } from "@heroicons/vue/outline";
</script>
