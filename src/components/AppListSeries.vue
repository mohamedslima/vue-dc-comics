<template>
  <div class="series_thumb">
    <div class="img_container">
      <img :src="seriesObj.thumb" alt="" />
    </div>
    <p>{{ seriesObj.price }}</p>
    <h4>{{ seriesObj.series }}</h4>
    <p>{{ seriesObj.type }}</p>
  </div>
</template>

<script>
export default {
  name: "AppListSeries",
  props: {
    seriesObj: Object,
  },
};
</script>

<style lang="scss" scoped>
div.series_thumb {
  width: calc(100% / 6 - 4px);
  padding: 2rem;
  div.img_container {
    img {
      width: 150px;
    }
  }
}
</style>
