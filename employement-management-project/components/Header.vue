<template>
  <header class="bg-white shadow mx-1 my-1 px-1 py-2 rounded-t-lg flex items-center justify-between">
    <h1 class="mx-4 text-xl font-semibold text-gray-900">Dashboard</h1>
    <div class="flex items-center gap-3">
      <div class="flex items-center border rounded-lg w-64 px-2">
        <svg 
          xmlns="http://www.w3.org/2000/svg" 
          class="h-5 w-5 text-gray-500 mr-2" 
          viewBox="0 0 20 20" 
          fill="currentColor"
        >
          <path 
            fill-rule="evenodd" 
            d="M9 3a6 6 0 105.293 10.293l3.707 3.707a1 1 0 001.414-1.414l-3.707-3.707A6 6 0 009 3zm4 6a4 4 0 11-8 0 4 4 0 018 0z" 
            clip-rule="evenodd"
          />
        </svg>
        <input
          type="text"
          placeholder="Quick Search..."
          class="w-full py-2 text-gray-700 focus:outline-none"
        />
      </div>

      <MailIcon class="h-8 rounded border  hover:bg-purple-700 hover:text-white border-black p-1" />

      <div
        class="w-32 h-8 rounded flex items-center justify-around text-gray-950 px-5 py-2 hover:bg-purple-700 hover:text-white  border border-black"
      >
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
