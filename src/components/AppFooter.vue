<template>
  <footer class="app-footer">{{ stats.active }} more to do, {{ stats.done }} done</footer>
</template>

<script lang="ts">
import { PropType, defineComponent } from 'vue';
import { Stats } from './../types/stats'


export default defineComponent({
  props: {
    stats: {
      type: Object as PropType<Stats>,
      required: true
    }
  }
})
</script>