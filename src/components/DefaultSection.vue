<template>
  <section class="section">
    <h3 class="section-title">{{ title }}</h3>
    <p class="section-description">{{ description }}</p>
  </section>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
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

  &-description {
    margin: 0 auto;
    font-size: 18px;
    width: auto;
    max-width: 680px;
    padding: 30px;
    border: 3px solid rgba(0, 200, 0, .3);
    border-radius: 20px;
  }
}
</style>
