<style lang="css">
  .category {
    width: 170px;
    height: 100%;
    float: left;
    color:  #cfcfcf;
  }
  .category-header,
  .category-footer {
    background-color: #12151a;
  }

  .category-content {
    background-color: #171a21;
    border-top: 1px solid #353535;
    border-bottom: 1px solid #353535;
  }

  .category-header {
    height: 38px;
  }

  .category-footer {
    height: 80px;
  }

  .category-content {
    height: calc(100% - 38px - 80px);
  }
</style>

<template lang="html">
  <div class="category">
    <category-header></category-header>
    <div class="category-content">
      <category-menu></category-menu>
      <category-menu></category-menu>
      <category-menu></category-menu>
    </div>
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
