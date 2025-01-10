<template>
  <div class="flex bg-gray-100">
    <aside class="flex w-64 bg-white rounded-lg shadow-md p-4">
      <SpeakerphoneIcon
        class="w-10 h-10 bg-purple-700 text-white rounded mr-4"
      />
      <div>
        <h2 class="font-semibold">Announcements</h2>
        <p>Stay updated with TurHr</p>
        <a href="#" class="underline text-purple-600 font-semibold"
          >Create Now</a
        >
      </div>
    </aside>
  </div>
  
</template>

<script setup>
import { SpeakerphoneIcon } from "@heroicons/vue/outline";
</script>
