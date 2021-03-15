<template>
   <div
    class="px-4 py-5 mx-auto sm:max-w-xl md:max-w-full lg:max-w-screen-xl md:px-24 lg:px-8"
  >
    <div class="relative flex grid items-center grid-cols-2 lg:grid-cols-3">
      <a
        href="/"
        aria-label="Company"
        title="Company"
        class="flex items-center lg:flex"
      >
        <svg
          class="w-8 text-teal-accent-400"
          viewBox="0 0 24 24"
          stroke-linejoin="round"
          stroke-width="2"
          stroke-linecap="round"
          stroke-miterlimit="10"
          stroke="currentColor"
          fill="none"
        >
          <rect x="3" y="1" width="7" height="12"></rect>
          <rect x="3" y="17" width="7" height="6"></rect>
          <rect x="14" y="1" width="7" height="6"></rect>
          <rect x="14" y="11" width="7" height="12"></rect>
        </svg>
        <span
          class="ml-2 text-xl font-bold tracking-wide text-gray-800 uppercase"
          >ALFATH</span
        >
      </a>
      <ul class="flex items-center lg:mx-auto space-x-8">
        <li>
          <a
            href="/"
            aria-label="Our product"
            title="Our product"
            class="font-medium tracking-wide text-gray-700 transition-colors duration-200 hover:text-gray-400"
            >Home</a
          >
        </li>
        <li>
          <a
            href="/"
            aria-label="Our product"
            title="Our product"
            class="font-medium tracking-wide text-gray-700 transition-colors duration-200 hover:text-gray-400"
            >Menu</a
          >
        </li>
        <li>
          <a
            href="/"
            aria-label="Product pricing"
            title="Product pricing"
            class="font-medium tracking-wide text-gray-700 transition-colors duration-200 hover:text-teal-accent-400"
            >Contact Us</a
          >
        </li>
      </ul>
      <a
        href="/"
        aria-label="Company"
        title="Company"
        class="flex items-center ml-auto lg:flex space-x-2"
      >
        <span
          class="ml-2 text-xl font-bold tracking-wide text-gray-800 uppercase"
          >Cart</span
        >
        <svg class="text-teal-accent-400" xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 24 24" fill="currentColor">
        <path d="M10 19.5c0 .829-.672 1.5-1.5 1.5s-1.5-.671-1.5-1.5c0-.828.672-1.5 1.5-1.5s1.5.672 1.5 1.5zm3.5-1.5c-.828 0-1.5.671-1.5 1.5s.672 1.5 1.5 1.5 1.5-.671 1.5-1.5c0-.828-.672-1.5-1.5-1.5zm1.336-5l1.977-7h-16.813l2.938 7h11.898zm4.969-10l-3.432 12h-12.597l.839 2h13.239l3.474-12h1.929l.743-2h-4.195z"/>
        </svg>
      </a>
    </div>
  </div>
</template>
