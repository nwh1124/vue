<template>
  <TitleBar />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import TitleBar from '../components/TitleBar.vue'

export default defineComponent({
  name: 'ArticleListPage',
  component: {
    TitleBar
  }
})
</script>

<style scoped>
</style>