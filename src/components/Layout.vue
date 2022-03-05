<template>
  <div class="nav-wrapper">
    <div class="content">
      <slot/>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'Layout.vue'
};
</script>

<style lang="scss" scoped>
.nav-wrapper {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.content {
  flex-grow: 1;
  overflow: auto;
}

</style>