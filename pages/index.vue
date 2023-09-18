<script setup lang="ts">
definePageMeta({
  documentDriven: false
})
</script>

<template>
  <div>
    <h1>This should give an "MFILE: too many open files" error during <code>pnpm generate</code> </h1>
    <ContentList path="/" v-slot="{ list }">
      <ul>
        <li v-for="entry in list" :key="entry._path">
          <NuxtLink :to="entry._path">
            {{ entry._path }}
          </NuxtLink>
        </li>
      </ul>
    </ContentList>
  </div>
</template>