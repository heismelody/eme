<template lang="html">
  <li class="browser-item">
    <p class="browser-item-title">{{ title }}</p>
    <p class="browser-item-content">{{ content }}</p>
    <p class="browser-item-time">{{ time }}</p>
  </li>
</template>

<script>
export default {
  name: 'browserItem',

  data() {
    return {
      title: 'Markdown Editor',
      content: `Basic useful feature listo here to load it`,
      time: '2018-7-7'
    }
  }
}
</script>

<style lang="css">
</style>
