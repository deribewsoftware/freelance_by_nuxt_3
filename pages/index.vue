<template>
  <div class="flex flex-col ">
    <Navbar/>
    <Hero/>
    <div class="container lg:grid lg:grid-cols-12 lg:gap-10 mt-12">
      <div class="col-span-3">
        <Sidebar/>
      </div>
<main class="w-full col-span-9 ">
  <Carousal/>
</main>
    </div>
   
  </div>
 
</template>

<script lang="ts" setup>

</script>

<style>
.container {
  padding: 0 50px;
}
</style>