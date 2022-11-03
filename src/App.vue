<script setup>
import { RouterView } from 'vue-router'
import { 
NLayout, 
NLayoutContent
} from 'naive-ui'

import Header from './layouts/Header.vue';
import Footer from './layouts/Footer.vue';
import Sidebar from './layouts/Sidebar.vue';
</script>

<template>
    <NLayout has-sider>
      <Sidebar />
      <NLayout style="min-height: 100vh;">
        <Header />
        <n-layout-content content-style="padding: 24px; padding-bottom: 70px">
          <RouterView />
        </n-layout-content>
        <Footer />
      </NLayout>
    </NLayout>
</template>

