<template>
  <div class="min-h-screen bg-gray-100 flex">
    <SideBar />
    <main class="flex-1">
      <Header class="px-1" />
      <div class="px-1">
        <Overview />
        <div class="py-1 grid grid-cols-1 lg:grid-cols-2 gap-1">
          <PerformanceTable />
          <StatisticsChart />
          <EmployeeTable />
        </div>
      </div>
    </main>
  </div>
</template>
