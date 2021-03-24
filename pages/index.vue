<template>
  <div class="container">
    <Navbar />
    <Header />
    <div class="w-full flex flex-col items-center mt-10">
      <h2 class="font-semibold text-3xl">Daftar Menu</h2>
      <div class="flex justify-between w-64 mt-10">
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
        class="w-40 mt-4"
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
        class="w-40 mt-4"
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

