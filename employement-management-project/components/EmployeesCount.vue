<template>
  <div class="bg-white p-6 rounded-lg shadow">
    <div class="flex justify-between items-center mb-4">
      <h3 class="font-semibold">Total Employees</h3>
      <DotsVerticalIcon class="w-5 h-5 text-gray-400" />
    </div>
    <div class="space-y-2">
      <div class="px-2 flex justify-between items-center bg-green-50 rounded-xl">
        <span class="text-2xl font-bold">150</span>
        <span class="text-green-500">+50</span>
        <p class="text-gray-500">Fulltime Employee</p>
      </div>
      <div class="px-2 flex justify-between items-center bg-orange-50 rounded-xl">
        <span class="text-2xl font-bold">50</span>
        <span class="text-orange-500">+10</span>
        <p class="text-gray-500">Freelance Employee</p>
      </div>
    </div>
  </div>
</template>
<script setup>
import { DotsVerticalIcon } from '@heroicons/vue/outline';

</script>
