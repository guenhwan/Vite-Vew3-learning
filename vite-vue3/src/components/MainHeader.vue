<script setup lang="ts">
  import { ref, reactive } from 'vue';

  interface Props {
    msg?: string;
    labels?: string[];
  }

  const props = withDefaults(defineProps<Props>(), {
    msg: 'hello',
    labels: () => ['one', 'two'],
  });

  const count = ref(0);
</script>

<template>
  <nav class="main-nav--bg">
    <div class="container main-nav">test</div>
    <font-awesome-layers full-width class="fa-4x">
      <font-awesome-icon :icon="['fas', 'envelope']" />
      <font-awesome-layers-text counter value="1" position="top-right" />
    </font-awesome-layers>
  </nav>
</template>

<style scoped lang="scss"></style>
