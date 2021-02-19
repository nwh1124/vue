<template>
  <section class="title-bar">
    <h1 class="container mx-auto">
      {{ title }}
    </h1>
  </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props:{
    msg:{
      type: String,
      required: true
    }
  },
  name: 'TitleBar'
})
</script>

<style>
</style>