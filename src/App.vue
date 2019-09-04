<template>
  <div id="app" class="app-body">
    <!--顶部header区域-->
    <header id="header" class="mui-bar mui-bar-nav">
      <h1 class="mui-title">车在哪</h1>
      <button class="mui-action-back mui-btn mui-btn-blue mui-btn-link mui-btn-nav mui-pull-left">
        <span class="mui-icon mui-icon-left-nav"></span>首页
      </button>
      <a class="mui-icon mui-icon-bars mui-pull-right"></a>
    </header>
    <!--中间router-view-->
    <router-view>
    </router-view>
    <!--底部tabBar区域-->
    <nav class="mui-bar mui-bar-tab">
      <router-link class="mui-tab-item" to="/map">
        <span class="mui-icon mui-icon-map"></span>
        <span class="mui-tab-label">地图</span>
      </router-link>
      <router-link class="mui-tab-item" to="/device">
        <span class="iconfont icon-shebei1"></span>
        <span class="mui-tab-label">设备</span>
      </router-link>
      <router-link class="mui-tab-item" to="/message">
        <span class="mui-icon mui-icon-email"><span class="mui-badge">9</span></span>
        <span class="mui-tab-label">消息</span>
      </router-link>
      <router-link class="mui-tab-item" to="/user">
        <span class="mui-icon mui-icon-contact"></span>
        <span class="mui-tab-label">我的</span>
      </router-link>
    </nav>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    //HelloWorld
  }
}
</script>

<style>
  .app-body {
    width: 100%;
    height: 100%;
    padding-top: 44px;
    padding-bottom: 53px;
  }
</style>
