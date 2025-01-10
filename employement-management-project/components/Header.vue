<template>
  <header class="bg-white shadow mx-1 my-1 px-1 py-2 rounded-t-lg flex items-center justify-between">
    <h1 class=" mx-4 text-xl font-semibold text-gray-900">Dashboard</h1>
    <div class="flex items-center gap-3">
      <input 
            type="text" 
            placeholder="Quick Search..." 
            class="px-4 py-2 border rounded-lg w-64"
          >
            <MailIcon class="h-8 rounded outline-double" />
          <div class="w-32 h-8 rounded flex items-center justify-around text-gray-950 px-5 py-2 hover:bg-purple-400 outline-double">
        <UserAddIcon class="w-5 h-5" />
        <button>
          Invite
        </button>
      </div>
     
    </div>
  </header>
</template>

<script setup>
import { MailIcon, UserAddIcon } from '@heroicons/vue/outline';

</script>
