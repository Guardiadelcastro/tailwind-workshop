<template>
  <header class="px-4 py-2 flex justify-between items-center md:px-6 md:py-4">
    <div
      class="px-3 py-1 flex items-center bg-emerald-200 text-emerald-900 rounded-full"
    >
      <svg
        class="h-6 w-6"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
        />
      </svg>
      <span class="ml-2 text-lg">Mail</span>
    </div>
    <div class="flex items-center space-x-2">
      <button
        class="p-1 rounded-full bg-transparent text-gray-600 focus:outline-none focus:bg-gray-100 focus:ring-2 focus:ring-gray-500 transition-colors ease-in-out duration-100 sm:hidden"
      >
        <svg
          class="h-6 w-6"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
          />
        </svg>
      </button>
      <div
        class="hidden sm:flex sm:items-center sm:rounded-full sm:bg-gray-200 sm:p-1 focus-within:ring-1 focus-within:ring-cyan-300"
      >
        <svg
          class="h-5 w-5 text-gray-500"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
          />
        </svg>
        <input
          class="bg-transparent px-2 border-0 focus:outline-none"
          type="text"
          aria-label="search emails"
          placeholder="Search..."
        />
      </div>
      <button
        class="p-1 rounded-full bg-cyan-200 text-cyan-700 hover:bg-cyan-200 focus:outline-none focus:ring-2 focus:ring-cyan-500 transition-colors ease-in-out duration-100"
      >
        <svg
          class="h-6 w-6"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
          />
        </svg>
      </button>
    </div>
  </header>
</template>

<script setup></script>
