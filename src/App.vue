<template>
  <lay-menu v-model:selected-key="selectedKey" v-model:open-keys="openKeys1">
    <lay-menu-item>首页</lay-menu-item>
    <lay-menu-item>首页</lay-menu-item>
    <lay-menu-item>首页</lay-menu-item>
    <lay-sub-menu>
      <template #title> 首页1 </template>
      <lay-menu-item>首页</lay-menu-item>
      <lay-sub-menu title="菜单">
        <template #title> 首页 </template>
        <lay-menu-item>首页</lay-menu-item>
        <lay-menu-item>首页</lay-menu-item>
        <lay-menu-item>首页</lay-menu-item>
      </lay-sub-menu>
      <lay-sub-menu title="菜单">
        <template #title> 首页 </template>
        <lay-menu-item>首页</lay-menu-item>
        <lay-menu-item>首页</lay-menu-item>
        <lay-menu-item>首页</lay-menu-item>
      </lay-sub-menu>
    </lay-sub-menu>
  </lay-menu>
</template>

<script>
import { ref } from 'vue';

export default {
  setup() {
    const selectedKey = ref('1');
    const openKeys1 = ref(['2']);
    return {
      selectedKey,
      openKeys1,
    };
  },
};
</script>
