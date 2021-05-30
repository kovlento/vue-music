<template>
  <div class="loading">
    <div class="loading-content">
      <img src="./loading.gif" alt="加载中..." width="24" height="24" />
      <p class="desc">{{ title }}</p>
    </div>
  </div>
</template>
<script>
export default {
  name: 'loading',
  data() {
    return {
      title: '正在加载...'
    }
  },
  methods: {
    setTitle(title) {
      this.title = title
    }
  }
}
</script>
<style lang="scss" scoped>
.loading {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate3d(-50%, -50%, 0);
  .loading-content {
    text-align: center;
    .desc {
      line-height: 20px;
      font-size: $font-size-small;
      color: $color-text-l;
    }
  }
}
</style>
