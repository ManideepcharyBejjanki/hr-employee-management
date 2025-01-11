<template>
   <div class="bg-white p-6 rounded-lg shadow">
    <div class="flex justify-between items-center mb-4">
      <h3 class="font-semibold">Today Used Devices</h3>
      <DotsVerticalIcon class="w-5 h-5 text-gray-400" />
    </div>
    <div class="flex justify-between items-center">
      <div class="relative w-32 h-32">
        <div class="text-center mt-12">
          <span class="text-3xl font-bold">100</span>
          <p class="text-sm text-gray-500">Overall</p>
        </div>
      </div>
      <div class="space-y-2">
        <div class="flex items-center gap-2">
          <span class="w-2 h-2 bg-teal-500 rounded-full"></span>
          <span class="text-black font-bold">80</span>
          <span class="text-gray-600">Macbook</span>
        </div>
        <div class="flex items-center gap-2">
          <span class="w-2 h-2 bg-orange-200 rounded-full"></span>
          <span class="text-black font-bold">13</span>
          <span class="text-gray-600">Keyboard</span>
        </div>
        <div class="flex items-center gap-2">
          <span class="w-2 h-2 bg-purple-600 rounded-full"></span>
          <span class="text-black font-bold">07</span>
          <span class="text-gray-600">Headphones</span>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { DotsVerticalIcon } from '@heroicons/vue/outline';

</script>
