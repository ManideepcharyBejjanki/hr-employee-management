<template>
  <div class="flex h-screen bg-gray-100">
    <aside class="w-64 bg-slate-100 shadow-md px-4">
      <div class="flex px-1 py-4 items-center justify-between mb-3">
        <h3 class="w-8 h-8 bg-purple-600 rounded-xl font-extrabold text-white flex items-center justify-center">
          H
        </h3>
        <h1 class="text-3xl font-bold text-gray-800">TurHR</h1>
        <UserIcon class="w-8 h-8 outline-dotted rounded-2xl"/>
      </div>
      <nav class="space-y-2">
        <a
          href="#"
          class="flex items-center gap-3 px-4 py-2 text-black font-semibold bg-white rounded-lg"
        >
          <HomeIcon class="w-5 h-5" />
          Dashboard
        </a>
        <template v-for="item in menuItems" :key="item.name">
          <a
            href="#"
            class="flex items-center gap-3 px-4 py-2 text-black font-semibold hover:bg-white rounded-lg"
          >
            <component :is="item.icon" class="w-5 h-5" />
            {{ item.name }}
          </a>
        </template>
        <div class="text-slate-400 font-semibold mx-2">TEAM MANAGEMENT</div>
        <template v-for="item in menuItems2" :key="item.name">
          <a
            href="#"
            class="flex items-center gap-3 px-4 py-2 text-black font-semibold hover:bg-white rounded-lg"
          >
            <component :is="item.icon" class="w-5 h-5" />
            {{ item.name }}
          </a>
        </template>
        <div>
          <Announcements />
        </div>
      </nav>
    </aside>
  </div>
</template>

<script setup lang="ts">
import {
  HomeIcon,
  CalendarIcon,
  CogIcon,
  BellIcon,
  QuestionMarkCircleIcon,
  DocumentIcon,
  CashIcon,
  DownloadIcon,
  UserGroupIcon,
  StarIcon,
  FlagIcon,
  UserIcon,
} from "@heroicons/vue/outline";

const menuItems = [
  { name: "Projects", icon: DocumentIcon, link: "#" },
  { name: "Calendar", icon: CalendarIcon, link: "#" },
  { name: "Leave Management", icon: CalendarIcon, link: "#" },
  { name: "Settings", icon: CogIcon, link: "#" },
  { name: "Notification", icon: BellIcon, link: "#" },
  { name: "Help & Center", icon: QuestionMarkCircleIcon, link: "#" },
];
const menuItems2 = [
  { name: "Performance", icon: StarIcon, link: "#" },
  { name: "Payrolls", icon: CashIcon, link: "#" },
  { name: "Invoices", icon: DownloadIcon, link: "#" },
  { name: "Employees", icon: UserGroupIcon, link: "#" },
  { name: "Recruitment & Hiring", icon: FlagIcon, link: "#" },
];
</script>
