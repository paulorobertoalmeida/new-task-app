<template>
  <button :style="{background: color }">{{text}}</button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
  }
};
</script>

<style scoped>
.btn {
@apply text-white bg-green-700 hover:bg-green-800 focus:ring-4 focus:ring-green-300 font-medium rounded-lg text-sm px-3 py-2 text-center inline-flex items-center  dark:bg-green-600 dark:hover:bg-green-700 dark:focus:ring-green-800
}
</style>