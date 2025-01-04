<template>
  <div id="basicLayout">
    <a-layout>
      <a-layout-header>
        <GlobalHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
      <a-layout-footer class="footer">
        <a href="https://codefather.cn" target="_blank"> 变成导航链接 </a>
      </a-layout-footer>
    </a-layout>
  </div>
</template>
<script setup lang="ts">
import GlobalHeader from "@/components/GlobalHeader.vue";
</script>
<style scoped>
#basicLayout .footer {
  background: #efefef;
  text-align: center;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  padding: 16px;
}

#basicLayout .content {
  padding: 20px;
  margin-bottom: 20px;
  background: linear-gradient(to right, #fefefe, #fff);
}
</style>
