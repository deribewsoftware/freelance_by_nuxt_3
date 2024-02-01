<script setup lang="ts">
const items = [
  {image:'https://picsum.photos/1920/1080?random=1'},
  {image:'https://picsum.photos/1920/1080?random=2'},
  {image:'https://picsum.photos/1920/1080?random=3'},
  {image:'https://picsum.photos/1920/1080?random=4'},
  {image:'https://picsum.photos/1920/1080?random=5'},
  {image:'https://picsum.photos/1920/1080?random=6'},
 
]
</script>

<template>
  <div class="w-full ">
    <UCarousel indicators v-slot="{ item }" :items="items" :ui="{ item: 'basis-1/3' }" class="overflow-hidden w-full " arrows>
      <Card :data="item"/>

  </UCarousel>
  </div>
</template>



