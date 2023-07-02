<template>
    <div>
  <div>
    <nav class="bg-white border-b border-gray-200">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between h-16">
          <div class="flex-shrink-0 flex items-center">
            <a href="/">
              <img class="h-8 w-auto" src="/logo.png" alt="Logo">
            </a>
          </div>
          <div class="hidden md:block">
            <div class="ml-4 flex items-center md:ml-6">
              <a href="/login" class="text-gray-600 hover:text-gray-900 px-3 py-2 rounded-md text-sm font-medium">Login</a>
              <a href="/signup" class="text-gray-600 hover:text-gray-900 px-3 py-2 rounded-md text-sm font-medium">Signup</a>
              <a href="/sell" class="text-gray-600 hover:text-gray-900 px-3 py-2 rounded-md text-sm font-medium">Sell</a>
              <a href="/buy" class="text-gray-600 hover:text-gray-900 px-3 py-2 rounded-md text-sm font-medium">Buy</a>
              <a href="/rent" class="text-gray-600 hover:text-gray-900 px-3 py-2 rounded-md text-sm font-medium">Rent</a>
            </div>
          </div>
          <div class="-mr-2 flex md:hidden">
            <button @click="toggleNav" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400 hover:text-gray-500 hover:bg-gray-100 focus:outline-none focus:bg-gray-100 focus:text-gray-500 transition duration-150 ease-in-out" aria-label="Main menu" aria-expanded="false">
              <svg class="h-6 w-6" stroke="currentColor" fill="none" viewBox="0 0 24 24">
                <path :class="{'hidden': isNavOpen, 'inline-flex': !isNavOpen}" class="inline-flex" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                <path :class="{'hidden': !isNavOpen, 'inline-flex': isNavOpen}" class="hidden" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
              </svg>
            </button>
          </div>
        </div>
      </div>
      <div :class="{'block': isNavOpen, 'hidden': !isNavOpen}" class="hidden md:hidden">
        <div class="px-2 pt-2 pb-3 sm:px-3">
          <a href="/login" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Login</a>
          <a href="/signup" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Signup</a>
          <a href="/sell" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Sell</a>
          <a href="/buy" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Buy</a>
          <a href="/rent" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-gray-900 hover:bg-gray-50 focus:outline-none focus:text-gray-900 focus:bg-gray-50 transition duration-150 ease-in-out">Rent</a>
        </div>
      </div>
      </nav>
      </div>
      </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isNavOpen: false,
      };
    },
  
    methods: {
      toggleNav() {
        this.isNavOpen = !this.isNavOpen;
      },
    },
  };
  </script>