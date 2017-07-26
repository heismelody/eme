<style lang="css">
  .category {
    width: 170px;
    height: 100%;
    float: left;
    background-color: #171a21;
  }
</style>

<template lang="html">
  <div class="category">
    <!-- <category-header></category-header> -->
    <category-menu></category-menu>
    <category-menu></category-menu>
    <category-menu></category-menu>
    <category-footer></category-footer>
  </div>
</template>

<script>
import categoryFooter from './categoryFooter';
import categoryHeader from './categoryHeader';
import categoryMenu from './categoryMenu';

export default {
  name: 'appCategory',

  components: {
    categoryHeader,
    categoryFooter,
    categoryMenu,
  }
}
</script>
