<template>
  <div>
    <header class="header">
      <h1 class="header-title">鶴姫</h1>
      <p class="header-subtitle">キャンプをより身近に。</p>
    </header>
    <Section
      title="鶴姫って？"
      description="鶴姫はあなたの自宅にキャンプ道具を貸し出します。キャンプ道具を揃えるのは敷居が高いですが、鶴姫を使うことで手軽に家でキャンプすることができます。"
    />
    <ListSection
      title="メリット"
      :items="items"
    />
    <div class="link">
      <p class="link-description">LINEでキャンプ道具の貸し出し予約ができます。以下のリンクから友達追加してください。</p>
      <a href="https://lin.ee/qNkgXqv"><img src="https://scdn.line-apps.com/n/line_add_friends/btn/ja.png" alt="友だち追加" height="36" border="0"></a>
    </div>
  </div>
</template>

<script>
import Section from './components/DefaultSection.vue'
import ListSection from './components/ListSection.vue'

export default {
  name: 'app',
  components: {
    Section,
    ListSection
  },
  data() {
    return {
      items: ["普段とは違った雰囲気を家で楽しめる", "高いキャンプ道具を買わなくてもいい", "LINEからキャンプ道具の貸し出し予約できる"]
    }
  }
}
</script>

<style lang="scss">
body {
  padding: 0;
  border: none;
  margin: 0 0 150px;
}

.header {
  padding: 150px 0;
  margin: 0 0 150px;
  text-align: center;
  background-color: rgba(0, 255, 0, .3);

  &-title {
    margin: 0 0 20px;
    font-size: 48px;
  }

  &-subtitle {
    margin: 0;
    font-size: 28px;
  }
}

.link {
  margin: 0 0 150px;
  text-align: center;

  &-description {
    font-size: 24px;
    margin: 0 0 20px;
  }
}
</style>
