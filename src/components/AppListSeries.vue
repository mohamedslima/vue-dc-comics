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
  text-align: center;
  div.img_container {
    width: 150px;
    height: 150px;
    contain: cover;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
  p {
    margin-top: 0.5rem;
    color: white;
  }
  h4 {
    color: white;
    font-size: 1.2rem;
  }
}
</style>
