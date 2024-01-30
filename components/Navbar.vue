<template>
  <header class="flex justify-around border-b-[1px] border-gray-200 dark:border-gray-700 ">
    <div class="">Nuxt Ui</div>
    <div class="">Nuxt Ui</div>
    <div class="">Nuxt Ui</div>
    <ClientOnly>
    <UButton
      :icon="isDark ? 'i-heroicons-moon-20-solid' : 'i-heroicons-sun-20-solid'"
      color="gray"
      variant="ghost"
      aria-label="Theme"
      @click="isDark = !isDark"
    />
    <template #fallback>
      <div class="w-8 h-8" />
    </template>
  </ClientOnly>
  </header>
</template>

<script lang="ts" setup>

const colorMode = useColorMode()
const isDark = computed({
  get () {
    return colorMode.value === 'dark'
  },
  set () {
    colorMode.preference = colorMode.value === 'dark' ? 'light' : 'dark'
  }
})

</script>

