<script setup>
import { ClockIcon, ListBulletIcon, ChartBarIcon } from '@heroicons/vue/24/outline'
const navItems = ['timeline', 'activities', 'progress']
</script>

<template>
<nav class="sticky bottom-0 z-10 border-b bg-gray-200 text-xl">
    <ul class="flex items-center justify-around border-t">
      <li v-for="page in navItems" :key="page" class="flex-1">
        <a :href="`#${page}`" class="flex flex-col items-center p-2 text-xs capitalize"
          ><ClockIcon v-if="page === 'timeline'" class="h-7 w-7" />
          <ListBulletIcon v-else-if="page === 'activities'" class="h-7 w-7" />
          <ChartBarIcon v-else class="h-7 w-7" />{{ page }}</a
        >
      </li>
    </ul>
  </nav>
</template>
