<template>
  <div class="col-span-1 lg:col-span-3 bg-white p-6 shadow rounded">
    <div class="flex items-center justify-between mb-2">
      <h2 class="text-lg font-semibold">All Employees</h2>
      <input 
            type="text" 
            placeholder="Search Employee" 
            class="px-3 py-1 border rounded-lg w-40"
          >
      <div
        class="w-30 h-10 flex items-center justify-between bg-white text-black px-5 py-2 rounded hover:bg-purple-500"
      >
        <UploadIcon class="w-5 h-5" />
        <button class="px-2">Export</button>
      </div>
    </div>

    <table class="w-full text-left text-gray-600">
      <thead>
        <tr class="border-b">
          <th class="py-2">Employee ID</th>
          <th class="py-2">Employee Name</th>
          <th class="py-2">Email</th>
          <th class="py-2">Role</th>
          <th class="py-2">Departments</th>
          <th class="py-2">Status</th>
          <th class="py-2">Action</th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="(employee, index) in employees"
          :key="index"
          class="border-b"
        >
          <td class="py-2">{{ employee.id }}</td>
          <td class="py-2">{{ employee.name }}</td>
          <td class="py-2">{{ employee.email }}</td>
          <td class="py-2">{{ employee.role }}</td>
          <td class="py-2">{{ employee.department }}</td>
          <td class="py-2">
            <span
              :class="
                employee.status === 'Full-time'
                  ? 'text-green-600'
                  : 'text-yellow-600'
              "
            >
              {{ employee.status }}
            </span>
          </td>
          <td class="py-2 flex items-center space-x-6">
            <EyeIcon class="w-4 h-4 text-gray-400" />
            <DotsVerticalIcon class="w-4 h-4 text-gray-400" />
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
import { DotsVerticalIcon, EyeIcon, UploadIcon } from "@heroicons/vue/outline";

const employees = [
  {
    id: "TUR871219",
    name: "Ahsan Tapadar",
    email: "ahsan.tur@gmail.com",
    role: "Sr UI/UX Designer",
    status: "Full-time",
    department: "Team Projects",
  },
  {
    id: "TUR85103",
    name: "Washi Bin M.",
    email: "wasih.tur@gmail.com",
    role: "Lead Product Designer",
    status: "Full-time",
    department: "Head of Projects",
  },
  {
    id: "TUR715481",
    name: "Koyes Ahmed",
    email: "koyes.tur@gmail.com",
    role: "Sr UX Designer",
    status: "Full-time",
    department: "Client & Team Work",
  },
  {
    id: "TUR016481",
    name: "Turja Sen Das",
    email: "Turja.tur@gmail.com",
    role: "Mid UI Designer",
    status: "Freelance",
    department: "Case Study",
  },
];
</script>
