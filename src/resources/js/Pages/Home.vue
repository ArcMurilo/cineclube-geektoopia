<template>
  <h1 class="text-center text-3xl font-bold text-gray-700">Cineclube - Geektoopia</h1>
  <blockquote class="text-center text-base mt-2 text-gray-700">{{ title }}</blockquote>

  <form class="mx-auto w-4/5 lg:w-1/2 shadow mt-8 rounded-md relative">
    <input type="text" placeholder="Pesquise um filme"
           class="text-xl p-3 text-gray-800 w-full border border-gray-400 rounded-md focus:outline-none focus:ring-1 focus:ring-gray-400">
    <svg class="h-8 w-8 text-gray-400 absolute inset-y-2.5 right-2" 
         xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
      <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
    </svg>
  </form>
</template>

<script>
export default {
  props: {
    title: String,
  }
}
</script>

<style>

</style>