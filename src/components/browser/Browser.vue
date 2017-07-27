<style lang="css">
  .browser {
    width: 270px;
    height: 100%;
    float: left;
    background-color: #f5f5f4;
  }

  .browser-header {
    height: 38px;
  }

  .browser-search {
    height: 40px;
  }
</style>

<template lang="html">
  <div class="browser">
    <div class="browser-header">

    </div>
    <div class="browser-search-container">
      <div class="browser-search">
        
      </div>
      <div class="browser-add">

      </div>
    </div>

    <ul class="browser-container" style="padding-left: 0px;">
      <browser-item></browser-item>
      <browser-item></browser-item>
      <browser-item></browser-item>
      <browser-item></browser-item>
      <browser-item></browser-item>
      <browser-item></browser-item>
    </ul>
  </div>
</template>

<script>
import browserItem from './BrowserItem';

export default {
  name: 'appBrowser',

  components: {
    browserItem,
  }
}
</script>
