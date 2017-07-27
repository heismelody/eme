<style lang="css">
  .browser {
    width: 270px;
    height: 100%;
    float: left;
    background-color: #f5f5f4;
  }

  .browser-header {
    height: 38px;
    padding: 7px;
  }

  .browser-search-container {
    border-bottom: 1px solid #cacaca;
  }

  .browser-search {
    height: 40px;
    padding: 5px 20px 5px 20px;
  }

  .browser-header-title {
    margin: 0px;
    color: #5d5d5d;
    font-size: 17px;
    text-align: center;
  }
</style>

<template lang="html">
  <div class="browser">
    <div class="browser-header">
      <p class="browser-header-title">All</p>
    </div>
    <div class="browser-search-container">
      <div class="browser-search">
        <search-box></search-box>
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
import searchBox from '../search-box';
import browserItem from './browser-item';

export default {
  name: 'appBrowser',

  components: {
    browserItem,
    searchBox
  }
}
</script>
