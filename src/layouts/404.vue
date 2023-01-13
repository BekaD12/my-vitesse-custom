<script setup lang="ts">
const router = useRouter()
const { t } = useI18n()
</script>

<template>
  <Header />
  <main p="x10 y50" text="center black dark:gray-200">
    <div text-4xl>
      <div i-carbon-warning inline-block />
    </div>
    <RouterView />
    <div>
      <button btn text-m m="3 t8" @click="router.back()">
        {{ t('button.back') }}
      </button>
    </div>
    <div class="mt-5 mx-auto text-center opacity-75 dark:opacity-50">
      [404 Layout]
    </div>
  </main>
</template>
