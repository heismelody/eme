<style lang="css">
  .browser-item {
    height: 90px;
    border-bottom: 0.5px solid #e6e6e6;
    padding: 15px;
    list-style: none;

    font-size: small;
    font-family: 'Roboto',arial,sans-serif;
    font-weight: normal;
    color: #545454;
    line-height: 1.4;
    word-wrap: break-word;
    text-align: left;

    p {
      margin: 0px;
    }

    &:hover {
      border-radius: 3px;
      background-color: #5391fc;
      cursor: pointer;

      color: #fff;
    }

    &:hover > .browser-item-title {
      color: #fff;
    }

    &:hover > .browser-item-content {
      color: #fff;
    }

    &:hover .browser-item-time {
      color: #fff;
    }

    .browser-item-title {
      color: #000;
      font-size: 15px;
      font-weight: bold;
      font-style: normal;
    }

    .browser-item-content {
      font-size: 13px;
    }

    .browser-item-time {
      color: #5391fc;
    }
  }
</style>

<template lang="html">
  <li class="browser-item">
    <p class="browser-item-title">{{ title }}</p>
    <p class="browser-item-content">
      <span class="browser-item-time">{{ time }}</span>
      &nbsp{{ content }}
    </p>
  </li>
</template>

<script>
export default {
  name: 'browserItem',

  data() {
    return {
      title: 'Markdown Editor',
      content: `Basic useful feature listo here to load it`,
      time: '4 hours ago'
    }
  }
}
</script>
