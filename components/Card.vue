<template>
  <div class="w-full  border border-slate-100  dark:border-slate-700 my-2 mx-4 flex flex-col bg-white dark:bg-slate-800 rounded-[5px]">
    <img v-if="data?.image" :src="data?.image" alt="photo" class="w-full rounded-t-[5px]"/>
    <div class="text-center p-2">Home rental</div>
    <div class="text-center p-2">Home rental</div>
    <div class="text-center p-2">Home rental</div>
    <div class="text-center p-2">Home rental</div>
    <hr>
    <div class="text-center p-2">Home rental</div>
  </div>
</template>

<script lang="ts" setup>
const props=defineProps({
  data:Object
})
</script>

<style>

</style>