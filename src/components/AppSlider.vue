<script>
export default {
  name: "AppSlider",
  props: {
    thumb: String,
    image: String,
    series: String,
    type: String
  }
}
</script>

<template>
  <div class="comic d-flex flex-column mx-1">
    <img :src="image" alt="" class="comic-cover">
    <h6 class="text-center ">{{ thumb }}</h6>
  </div>
</template>

<style lang="scss">
.comic {
  width: calc(100% / 6  / 6 * 5);
}

.comic-cover {
  width: 100%;
  margin-bottom: 1em;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  object-position: top;
}

</style>


