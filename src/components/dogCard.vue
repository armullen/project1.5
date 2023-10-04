<script lang="ts" setup>

defineProps({
    dog: Object,
    required: true
})
</script>

<template>
    <div class="dog-card">
      <h2>{{ dog.name }}</h2>
      <h5>{{ dog.breed }}</h5>
    </div>
</template>

<style scoped>
</style>
```