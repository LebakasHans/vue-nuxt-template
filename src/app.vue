<script setup lang="ts">
const test = ref('test');
if (test.value === 'test') {
  console.warn('client');
}
else {
  console.warn('server');
}
</script>

<template>
  <NuxtLayout>
    <NuxtPage />
  </NuxtLayout>
</template>
