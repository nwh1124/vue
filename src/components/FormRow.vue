<template>
  <div class="form-row flex flex-col md:flex-row">
    <div class="w-32 flex justify-center">
      <span class="lg:flex md:items-center lg:w-28">{{title}}</span>
    </div>
    <div class="lg:flex-grow">
      <slot>        
      </slot>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    title: {
      type: String,
      required: true
    }
  },
  name: 'FormRow'
})
</script>

<style lang="postcss">
.form-row-select {
  @apply w-full rounded-sm;
}

.form-row-input{
  @apply w-full rounded-sm;
}

textarea.form-row-input{
  min-height: theme('spacing.72');
}

.form-row + .form-row {
  @apply mt-2;
}
</style>

<style scoped>
</style>