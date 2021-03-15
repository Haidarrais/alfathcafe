<template>
  <div class="container">
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
          <svg
            class="text-teal-accent-400"
            xmlns="http://www.w3.org/2000/svg"
            width="30"
            height="30"
            viewBox="0 0 24 24"
            fill="currentColor"
          >
            <path
              d="M10 19.5c0 .829-.672 1.5-1.5 1.5s-1.5-.671-1.5-1.5c0-.828.672-1.5 1.5-1.5s1.5.672 1.5 1.5zm3.5-1.5c-.828 0-1.5.671-1.5 1.5s.672 1.5 1.5 1.5 1.5-.671 1.5-1.5c0-.828-.672-1.5-1.5-1.5zm1.336-5l1.977-7h-16.813l2.938 7h11.898zm4.969-10l-3.432 12h-12.597l.839 2h13.239l3.474-12h1.929l.743-2h-4.195z"
            />
          </svg>
        </a>
        <div class="ml-auto lg:hidden">
          <button
            aria-label="Open Menu"
            title="Open Menu"
            class="p-2 -mr-1 transition duration-200 rounded focus:outline-none focus:shadow-outline hover:bg-deep-teal-accent-50 focus:bg-deep-teal-accent-50"
            @click="isMenuOpen = true"
          >
            <svg class="w-5 text-gray-600" viewBox="0 0 24 24">
              <path
                fill="currentColor"
                d="M23,13H1c-0.6,0-1-0.4-1-1s0.4-1,1-1h22c0.6,0,1,0.4,1,1S23.6,13,23,13z"
              ></path>
              <path
                fill="currentColor"
                d="M23,6H1C0.4,6,0,5.6,0,5s0.4-1,1-1h22c0.6,0,1,0.4,1,1S23.6,6,23,6z"
              ></path>
              <path
                fill="currentColor"
                d="M23,20H1c-0.6,0-1-0.4-1-1s0.4-1,1-1h22c0.6,0,1,0.4,1,1S23.6,20,23,20z"
              ></path>
            </svg>
          </button>
          <div v-if="isMenuOpen" class="absolute top-0 left-0 w-full">
            <div class="p-5 bg-white border rounded shadow-sm">
              <div class="flex items-center justify-between mb-4">
                <div>
                  <a
                    href="/"
                    aria-label="Company"
                    title="Company"
                    class="inline-flex items-center"
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
                      >Company</span
                    >
                  </a>
                </div>
                <div>
                  <button
                    aria-label="Close Menu"
                    title="Close Menu"
                    class="p-2 -mt-2 -mr-2 transition duration-200 rounded hover:bg-gray-200 focus:bg-gray-200 focus:outline-none focus:shadow-outline"
                    @click="isMenuOpen = false"
                  >
                    <svg class="w-5 text-gray-600" viewBox="0 0 24 24">
                      <path
                        fill="currentColor"
                        d="M19.7,4.3c-0.4-0.4-1-0.4-1.4,0L12,10.6L5.7,4.3c-0.4-0.4-1-0.4-1.4,0s-0.4,1,0,1.4l6.3,6.3l-6.3,6.3 c-0.4,0.4-0.4,1,0,1.4C4.5,19.9,4.7,20,5,20s0.5-0.1,0.7-0.3l6.3-6.3l6.3,6.3c0.2,0.2,0.5,0.3,0.7,0.3s0.5-0.1,0.7-0.3 c0.4-0.4,0.4-1,0-1.4L13.4,12l6.3-6.3C20.1,5.3,20.1,4.7,19.7,4.3z"
                      ></path>
                    </svg>
                  </button>
                </div>
              </div>
              <nav>
                <ul class="space-y-4">
                  <li>
                    <a
                      href="/"
                      aria-label="Our product"
                      title="Our product"
                      class="font-medium tracking-wide text-gray-700 transition-colors duration-200 hover:text-teal-accent-400"
                      >Home</a
                    >
                  </li>
                  <li>
                    <a
                      href="/"
                      aria-label="Our product"
                      title="Our product"
                      class="font-medium tracking-wide text-gray-700 transition-colors duration-200 hover:text-teal-accent-400"
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
                  <li>
                    <a
                      href="/"
                      aria-label="Sign in"
                      title="Sign in"
                      class="font-medium tracking-wide text-gray-700 transition-colors duration-200 hover:text-teal-accent-400"
                      >Sign in</a
                    >
                  </li>
                  <li>
                    <a
                      href="/"
                      class="inline-flex items-center justify-center w-full h-12 px-6 font-medium tracking-wide text-white transition duration-200 rounded shadow-md bg-teal-accent-400 hover:bg-teal-700 focus:shadow-outline focus:outline-none"
                      aria-label="Sign up"
                      title="Sign up"
                    >
                      Sign up
                    </a>
                  </li>
                </ul>
              </nav>
            </div>
          </div>
        </div>
      </div>
    </div>
    <Header />
    <div class="w-full flex flex-col items-center mt-10">
      <h2 class="font-semibold text-3xl">Daftar Menu</h2>
      <div class="flex justify-between w-64">
        <div
          class="font-bold px-10 py-2 cursor-pointer"
          v-bind:class="isDrinks ? 'active' : ''"
          @click="isDrinks = true"
        >
          Drinks
        </div>
        <div
          class="font-bold px-10 py-2 cursor-pointer"
          v-bind:class="isDrinks ? '' : 'active'"
          @click="isDrinks = false"
        >
          Foods
        </div>
      </div>
      <div
        class="w-40 mt-2"
        v-bind:class="isDrinks ? 'flex justify-between ' : 'hidden'"
      >
        <div
          v-bind:class="isChildren ? 'activeChildren' : ''"
          @click="isChildren = true"
          class="text-sm cursor-pointer"
        >
          Hot
        </div>
        <div
          v-bind:class="isChildren ? '' : 'activeChildren'"
          @click="isChildren = false"
          class="text-sm cursor-pointer"
        >
          Cold
        </div>
      </div>
      <div
        class="w-40 mt-2"
        v-bind:class="isDrinks ? 'hidden' : 'flex  justify-between '"
      >
        <div
          v-bind:class="isChildren ? 'activeChildren' : ''"
          @click="isChildren = true"
          class="text-sm cursor-pointer"
        >
          Snack
        </div>
        <div
          v-bind:class="isChildren ? '' : 'activeChildren'"
          @click="isChildren = false"
          class="text-sm cursor-pointer"
        >
          Meals
        </div>
      </div>
      <Content />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
      isDrinks: true,
      isChildren: true,
    };
  },
};
</script>
<style lang="postcss">
.active {
  @apply bg-black text-white rounded-3xl;
}
.activeChildren {
  border-bottom: 2px solid black;
  font-weight: 500;
}
</style>
