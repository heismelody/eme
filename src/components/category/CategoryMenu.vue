<style lang="css">
  .category-menu svg{
    width: 20px;
    fill: #cfcfcf;
  }

  .menu-title:hover,
  .menu-subtitle:hover {
    background-color: #393f50;
    color: #c7c7c7;
    cursor: pointer;
  }

  .menu-title {
    color: #aaabae;
  }

  .menu-subtitle {
    color: #818386;
    list-style: none;
  }
</style>

<template lang="html">
  <div class="category-menu">
    <div class="menu-title">
      <svg-icon name="menuPaper"></svg-icon>
      <span>Notes</span>
    </div>
    <div class="menu-subtitle-container">
      <ul>
        <li class="menu-subtitle">yestarday</li>
        <li class="menu-subtitle">today</li>
        <li class="menu-subtitle">tomorrow</li>
      </ul>
    </div>
    <!--
    <svg-icon name="menuBook"></svg-icon>
    <svg-icon name="menuTags"></svg-icon> -->
  </div>
</template>

<script>
import SvgIcon from 'components/svg-icon'

export default {
  name: 'categoryMenu',

  components: {
    SvgIcon,
  }
}
</script>
