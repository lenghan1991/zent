<template>
  <div class="app">
    <div class="page-header">
      header
    </div>
    <div class="main-content">
      <div class="page-container clearfix">
        <side-nav :data="navConfig['zh-CN']" base="/component"></side-nav>
        <div class="page-content">
          <router-view></router-view>
          <footer-nav></footer-nav>
        </div>
      </div>
    </div>
    <div class="page-footer">
      footer
    </div>
  </div>
</template>

<script>
import 'highlight.js/styles/color-brewer.css';
import navConfig from '../nav.config.js';

export default {
  data() {
    return {
      navConfig: navConfig
    };
  }
};
</script>

<style lang="css">
  @import '../assets/docs.css';
  @import '../assets/react-docs.css';
</style>
