<template>
  <section class="section">
    <div class="columns is-mobile is-multiline is-centered">
      <div class="column is-mobile is-multiline is-centered is-narrow">
        <div class="icon">
          <img
            src="~assets/manaty.jpg"
            alt="icon">
        </div>
      </div>
      <div class="column is-mobile is-multiline is-centered is-narrow">
        <div class="text-area">
          <h1>Tanaka Mana</h1>
          <p>1995年生まれの新卒1年目。</p>
          <p>外資コンサルティングファームのエンジニアとして働いている。</p>
        </div>
        <div class="sns-area">
          <img
            src="~assets/twitter-icon.svg"
            alt="twitter">
          <img
            src="~assets/qiita-icon.png"
            alt="qiita">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '@/components/Logo'

export default {
  name: 'HomePage',
  components: { Logo }
}
</script>

<style scoped lang="scss">
section {
  background-color: #f08080;
  color: #ffffff;
  height: calc(100vh - 40px);
  h1 {
    font-weight: bold;
  }
}
.catch {
  text-align: center;
}
.icon {
  height: 120px;
  width: 120px;
  img {
    height: 100%;
    border-radius: 100px;
  }
}
.text-area {
  margin-bottom: 10px;
}
.sns-area {
  img {
    height: 40px;
    width: 40px;
  }
}
</style>
