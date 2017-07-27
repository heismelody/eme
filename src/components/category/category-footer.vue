<style lang="css">
  .category-footer svg {
    width: 10px;
    fill: #cfcfcf;
  }

  .category-footer p{
    margin-top: 0px;
    margin-bottom: 0px;
  }

  .category-footer-name {
    float: left;
    margin-right: 20px;
    margin-left: 10px;
  }

  .category-footer-user {
    height: 20px;
    padding-left: 15px;
    padding-top: 10px;
    padding-right: 25px;
  }

  .category-footer-more {
    float: right;
    padding-top: 1px;
  }

  .category-footer-time {
    margin-left: 20px;
    margin-right: 20px;
    color: #818386;
    text-align: center;
    font-size: 12px;
  }
</style>

<template lang="html">
  <div class="category-footer">
    <div class="category-footer-user">
      <p class="category-footer-name">{{ name }}</p>
      <div class="category-footer-more">
        <svg-icon name='down'></svg-icon>
      </div>
    </div>
    <p class="category-footer-time">{{ time }}</p>
  </div>
</template>

<script>
import SvgIcon from 'components/svg-icon'

export default {
  name: 'categoryFooter',

  data() {
    return {
      name: 'sindresorhus',
      time: '0000/00/00 00:00:00'
    }
  },

  components: {
    SvgIcon,
  },

  created() {
    this.clock();
  },

  methods: {
    clock() {
      let self = this;

      let date = new Date();
      let y = date.getUTCFullYear();
      let mon = date.getUTCMonth()
      let d = date.getUTCDate();
      let h = date.getHours();
      let m = date.getMinutes();
      let s = date.getSeconds();
      m = this.checkTime(m);
      s = this.checkTime(s);
      this.time = `${y}/${mon}/${d} ${h}:${m}:${s}`;

      setTimeout(this.clock, 500);
    },

    checkTime(i) {
      return (i < 10) ? ("0" + i) : i;
    },

  }
}
</script>
