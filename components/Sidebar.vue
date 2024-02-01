<template>
  <aside class="sticky h-screen w-72">
    <div class="h-full w-full items-start px-10 overflow-y-auto flex flex-col gap-10 py-10 border-r-[1px]  dark:border-slate-700">
     <UAccordion
   
      :items="items" 
      :ui="{ wrapper: 'flex flex-col w-full' }
      
      ">
<template #item="{ item }">
      <p class="italic text-gray-900 dark:text-white text-center">
        {{ item.alist }}
      </p>
    </template>

   <template #default="{ item, index, open }">
    <UButton color="gray" variant="ghost" class="border-b border-gray-200 dark:border-gray-700" :ui="{ rounded: 'rounded-none', padding: { sm: 'p-3' } }">
        

        <span class="truncate">{{ item.label }}</span>

        <template #trailing>
          <UIcon
            name="i-heroicons-chevron-right-20-solid"
            class="w-5 h-5 ms-auto transform transition-transform duration-200"
            :class="[open && 'rotate-90']"
          />
        </template>
      </UButton>
   </template>


     </UAccordion>
    </div>
  </aside>
</template>

<script lang="ts" setup>
const items = [
  {
    label:"Getting Started",
    alist:"Getting Started lists",
   content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed neque elit, tristique placerat feugiat ac, facilisis vitae arcu. Proin eget egestas augue. Praesent ut sem nec arcu pellentesque aliquet. Duis dapibus diam vel metus tempus vulputate.'
  },
  {
    label:"Components",
    alist:"list of components",
    
    content: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed neque elit, tristique placerat feugiat ac, facilisis vitae arcu. Proin eget egestas augue. Praesent ut sem nec arcu pellentesque aliquet. Duis dapibus diam vel metus tempus vulputate.'

  }
]
</script>

<style>

</style>