<script setup lang="ts">
const { page } = useContent()
</script>

<template>
  <div>
    {{ page._path }}
  </div>
</template>