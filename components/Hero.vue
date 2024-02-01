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
  <div class="w-full text-center items-center flex justify-around h-screen">

    <div class="flex flex-col gap-2">
      <h1 class="text-6xl font-bold">Welcome to Hero Homes - Where Your Comfort Finds Its Address!</h1>
      <h1 class="text-4xl font-semibold mt-2">🏡 Discover Your Haven:</h1>
      <p class="py-2 px-20 text-base text-slate-500 dark:text-slate-400 justify-start text-start">Welcome to the epitome of luxurious living! Hero Homes invites you to experience a seamless blend of elegance and modernity. Our curated selection of premium homes ensures that you not only find a house but a haven that resonates with your lifestyle.</p>
    </div>
    <div class="w-1/3">
      <img src="https://freepngimg.com/thumb/home/150412-home-free-hd-image.png" alt="logo"/>
    </div>
    
  </div>
</template>



