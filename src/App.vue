<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
// import HelloWorld from './components/HelloWorld.vue'
import { releaseDate } from './utils/release'

if (process.env.NODE_ENV !== 'development' && releaseDate.date != null && releaseDate.date !== '') {
  console.log('项目发布日期：', releaseDate.date)
}

const host = location.host

</script>

<template>
  <!-- xuxiaowei-tools.gitee.io -->
  <component :is="'script'" v-if="host === 'xuxiaowei-tools.gitee.io'">
    var _hmt = _hmt || [];
    (function() {
    var hm = document.createElement("script");
    hm.src = "https://hm.baidu.com/hm.js?fe43c611db42a5c57941f6c4c99e3f48";
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(hm, s);
    })();
  </component>

  <!-- xuxiaowei-tools.gitlab.io -->
  <component :is="'script'" v-if="host === 'xuxiaowei-tools.gitlab.io'">
    var _hmt = _hmt || [];
    (function() {
    var hm = document.createElement("script");
    hm.src = "https://hm.baidu.com/hm.js?aff1e8e26cdd5ec3407bcc223abe3c69";
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(hm, s);
    })();
  </component>

  <!-- xuxiaowei-tools.github.io -->
  <component :is="'script'" v-if="host === 'xuxiaowei-tools.github.io'">
    var _hmt = _hmt || [];
    (function() {
    var hm = document.createElement("script");
    hm.src = "https://hm.baidu.com/hm.js?f7a91487a3aab43e801945044060e488";
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(hm, s);
    })();
  </component>

  <!-- tools.xuxiaowei.com.cn -->
  <component :is="'script'" v-if="host === 'tools.xuxiaowei.com.cn'">
    var _hmt = _hmt || [];
    (function() {
    var hm = document.createElement("script");
    hm.src = "https://hm.baidu.com/hm.js?fe8e32733f88dbb086002fdedf7bee8b";
    var s = document.getElementsByTagName("script")[0];
    s.parentNode.insertBefore(hm, s);
    })();
  </component>

  <el-row justify="space-evenly">
    <el-col :span="22" class="text-center">
      <router-link to="/">Home</router-link>
      <el-divider direction="vertical" />
      <router-link to="/region">省市区</router-link>
      <el-divider direction="vertical" />
      <router-link to="/editor/toast-ui">ToastUi</router-link>
      <el-divider direction="vertical" />
      <router-link to="/editor/wangeditor">WangEditor</router-link>
      <el-divider direction="vertical" />
      <router-link to="/password">Password</router-link>
      <el-divider direction="vertical" />
      <router-link to="/uuid">UUID</router-link>
      <el-divider direction="vertical" />
      <router-link to="/encryption/BCrypt">BCrypt</router-link>
      <el-divider direction="vertical" />
      <router-link to="/encryption/RSA">RSA</router-link>
      <el-divider direction="vertical" />
      <router-link to="/encryption/AES">AES</router-link>
      <el-divider direction="vertical" />
      <router-link to="/encryption/JWT">JWT</router-link>
      <el-divider direction="vertical" />
      <router-link to="/encryption/MD5">MD5</router-link>
      <el-divider direction="vertical" />
      <router-link to="/timestamp">TimeStamp</router-link>
      <el-divider direction="vertical" />
      <router-link to="/ip">IP</router-link>
      <el-divider direction="vertical" />
      <router-link to="/idCard">IdCard</router-link>
      <el-divider direction="vertical" />
      <router-link to="/docker/images/migrate">Docker Images 迁移</router-link>
      <el-divider direction="vertical" />
      <router-link to="/about">About</router-link>

    </el-col>
  </el-row>
  <router-view/>
</template>

<style scoped>

</style>
