<script setup lang="ts">
import { Edit, Search } from '@element-plus/icons-vue'
import TestComponent from '@/components/TestComponent.vue'
</script>

<template>
  <el-button type="primary" :icon="Edit">Primary</el-button>
  <el-button type="success" size="small" :icon="Search">Primary</el-button>

  <el-pagination :page-size="100" layout="total, prev, pager, next" :total="1000" />
  <TestComponent></TestComponent>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
