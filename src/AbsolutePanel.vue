<template>
  <!-- 绝对定位面板 可以自动适应内容大小 -->
  <div class="container" :style="{ 'top': top, 'left': left, 'right': right, 'bottom': bottom, 'z-index': zIndex }">
    <div class="wrapper">
      <slot></slot>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'AbsolutePanel',
    props: {
      top: {
        type: String,
        default: 'auto',
        required: false
      },
      left: {
        type: String,
        default: 'auto',
        required: false
      },
      right: {
        type: String,
        default: 'auto',
        required: false
      },
      bottom: {
        type: String,
        default: 'auto',
        required: false
      },
      zIndex: {
        type: Number,
        default: 9,
        required: false
      }
    }
  }
</script>

<style scoped>
  .container {
    position: absolute;
    margin: 0;
    padding: 0;
    z-index: 9;
  }

  .wrapper {
    position: relative;
    width: 100%;
    height: 100%;
  }
</style>
