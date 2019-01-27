<template>
  <div>
    <nav
      class="navbar"
      role="navigation"
      aria-label="main navigation"
    >
      <div class="navbar-brand">
        <a
          role="button"
          class="navbar-burger burger"
          aria-label="menu"
          aria-expanded="false"
          data-target="navbarBasicExample"
        >
          <span
            aria-hidden="true"/>
          <span
            aria-hidden="true"/>
          <span
            aria-hidden="true"/>
        </a>
      </div>

      <div
        id="navbarBasicExample"
        class="navbar-menu">
        <div class="navbar-end">
          <template
            v-for="(item, key) of items"
          >
            <nuxt-link
              :key="key"
              :to="item.to"
              class="navbar-item">
              {{ item.title }}
            </nuxt-link>
          </template>
        </div>
      </div>
    </nav>
    <nuxt />
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: 'Profile', to: { name: 'index' } },
        { title: 'Prototypes', to: { name: 'prototypes' } },
        { title: 'Works', to: { name: 'works' } },
        { title: 'Skills', to: { name: 'skills' } }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
nav {
  background-color: #f8f8f7;
  .navbar-item {
    color: #2c1814;
  }
}
</style>
