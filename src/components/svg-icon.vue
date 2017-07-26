<template>
  <span
    class="svg-icon"
    v-html="icon">
  </span>
</template>

<script>
  import pencil from 'src/svg/pencil.svg'
  import alignHorizontalMiddle from 'src/svg/align-horizontal-middle.svg'
  import eye from 'src/svg/eye.svg'
  import arrowLeft from 'src/svg/arrow-left.svg'
  import arrowRight from 'src/svg/arrow-right.svg'
  import settings from 'src/svg/settings.svg'
  import menuBook from 'src/svg/book.svg'
  import menuPaper from 'src/svg/file-o.svg'
  import menuTags from 'src/svg/tags.svg'

  const icons = {
    pencil,
    alignHorizontalMiddle,
    eye,
    arrowRight,
    arrowLeft,
    settings,
    menuBook,
    menuPaper,
    menuTags,
  }

  export default {
    props: {
      name: {
        required: true,
        type: String
      }
    },
    computed: {
      icon() {
        return icons[this.name]
      }
    }
  }
</script>
