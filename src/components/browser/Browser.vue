<style lang="css">
  .browser {
    width: 270px;
    height: 100%;
    float: left;
    background-color: #f5f5f4;
  }
</style>

<template lang="html">
  <div class="browser">
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
