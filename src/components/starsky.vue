<template>
  <div
    class="star"
    v-for="i in item.count"
    :key="i"
    :style="{
      background:
        'rgba(' +
        Math.floor(Math.random() * (255 - item.color.r) + item.color.r) +
        ',' +
        Math.floor(Math.random() * (255 - item.color.g) + item.color.g) +
        ',' +
        Math.floor(Math.random() * (255 - item.color.b) + item.color.b) +
        ',' +
        Math.random() +
        ')',
      top: Math.random() * 100 + 'vh',
      left: Math.random() * 100 + 'vw',
      transform:
        'scale(' + (Math.random() * (item.big - item.scale) + item.scale) + ')',
      filter: 'blur(' + item.blur + 'px)',
      width: item.size + 'px',
      height: item.size + 'px'
    }"
  ></div>
</template>

<script>
export default {
  props: { item: Object }
};
</script>

<style>
.star {
  position: absolute;

  border-radius: 50%;
}
</style>
