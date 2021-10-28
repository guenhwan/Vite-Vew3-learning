<template>
  <aside class="sidebar">
    <div class="sidebar-head">
      <a href="/" class="logo-wrapper" title="Home">{{ msg }}</a>
      <!-- <button @click="" class="">이동</button> -->
    </div>
    <div class="sidebar-body"></div>
    <div class="sidebar-footer"></div>
  </aside>
</template>

<script setup lang="ts">
  import { ref, reactive } from 'vue';

  defineProps<{ msg: string }>();

  const count = ref(0);
</script>

<style scoped lang="scss">
  .sidebar {
    position: -webkit-sticky;
    position: sticky;
    top: 0;
    height: 100%;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
    -ms-flex-direction: column;
    flex-direction: column;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    background-color: #0061f7 !important;
    width: 253px;
    padding: 20px 15px 37px 20px;
    -webkit-transition: 0.5s all;
    -o-transition: 0.5s all;
    transition: 0.5s all;
    min-height: 100vh;
  }
  .sidebar-head {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -webkit-box-pack: justify;
    -ms-flex-pack: justify;
    justify-content: space-between;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    padding-bottom: 20px;
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  }
</style>
