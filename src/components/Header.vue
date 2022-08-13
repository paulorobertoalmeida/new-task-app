<script >
import Button from "./Button.vue";

export default {
  name: "Header",

  props: {
    title: String,
  },
  components: {
    Button,
  },
};
</script>

<template>
  <header class="header">
    <div>
      <div
        class="
          bg-white
          shadow-md
          border border-gray-200
          rounded-lg
          max-w-sm
          mb-5
        "
      >
        <div class="p-5 flex justify-between ">
          <a href="#">
            <h5 class="text-gray-900 font-bold text-2xl tracking-tight mb-2">
              {{ title }}
            </h5>
          </a>
          <Button />
          </div>
          <div class="p-5">
          <p class="font-normal text-gray-700 mb-3">
            Here are the biggest enterprise technology acquisitions of 2021 so
            far, in reverse chronological order.
          </p>
        </div>
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  @apply mt-5 max-w-lg mx-auto;
}
</style>
