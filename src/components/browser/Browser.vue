<style lang="css">
  .browser {
    width: 270px;
    height: 100%;
    float: left;
    background-color: #f5f5f4;
  }

  .browser-container li {
    height: 90px;
    border-bottom: 0.5px solid #e6e6e6;
    text-align: center;
    padding: 15px;
    list-style: none;
  }

  .browser-container li:hover {
    border-radius: 3px;
    color: #fff;
    background-color: #5391fc;
    cursor: pointer;
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
