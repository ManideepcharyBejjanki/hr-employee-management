<template>
  <div class="bg-white p-6 shadow rounded">
    <h2 class="text-lg font-semibold mb-4">Employee Performance Ratings</h2>
    <ul>
      <li
        v-for="(employee, index) in employees"
        :key="index"
        class="flex justify-between py-2 border-b"
      >
        <span>{{ employee.name }}</span>
        <span>{{ employee.rating }}%</span>
      </li>
    </ul>
  </div>
</template>

<script setup>
const employees = [
  {
    id: "TUR871219",
    name: "Ahsan Tapadar",
    role: "Sr UI/UX Designer",
    rating: 98,
    status: "Full-time",
  },
  {
    id: "TUR85103",
    name: "Washi Bin M.",
    role: "Lead Product Designer",
    rating: 95,
    status: "Full-time",
  },
  {
    id: "TUR715481",
    name: "Koyes Ahmed",
    role: "Sr UX Designer",
    rating: 92,
    status: "Full-time",
  },
  {
    id: "TUR016481",
    name: "Turja Sen Das",
    role: "Mid UI Designer",
    rating: 89,
    status: "Freelance",
  },
];
</script>
