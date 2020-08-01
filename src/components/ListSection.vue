<template>
  <section class="section">
    <h3 class="section-title">{{ title }}</h3>
    <ul class="section-list">
      <li v-for="(item, index) in items" :key="index" class="section-item">・{{ item }}</li>
    </ul>
  </section>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    items: {
      type: Array,
      required: true
    }
  }
}
</script>

<style scoped lang="scss">
.section {
  margin: 0 0 150px;
  padding: 0 20px;
  text-align: center;

  &-title {
    margin: 0 0 50px;
    font-size: 38px;
  }

  &-list {
    margin: 0 auto;
    width: auto;
    max-width: 680px;
    font-size: 18px;
    padding: 30px;
    border: 3px solid rgba(0, 200, 0, .3);
    border-radius: 20px;
  }

  &-item {
    text-align: left;
    margin: 0 0 10px;
    list-style: none;
  }
}
</style>
