<script setup lang="ts">
const props = defineProps<{
  greeting: string;
}>();

const count = ref<number>(0);
</script>

<template>
  <div class="hello-world">
    <h1>{{ props.greeting }}</h1>
    <p>This is a sample component</p>
    <button @click="count++">
      Clicked {{ count }} times
    </button>
  </div>
</template>

<style scoped>
.hello-world {
  padding: 20px;
  border: 1px solid #eee;
  border-radius: 8px;
  margin: 20px 0;
}
</style>
