<template>
    <div class="Header">
      <header>
        <div class="navbar">
          <div class="container">
            <div class="navbar-content">
              <div class="logo">Blog</div>
              <ul class="navbar-list">
                <li class="navbar-item" v-for="link in links" :key="link.title">
                  <nuxt-link class="navbar-link" :title="link.title" :to="link.url">{{ link.title }}</nuxt-link>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </header>
    </div>
</template>

<script>
    export default {
        name: "Header",
        components: {},
        data() {
            return {
              links: [
                { title: 'Home', url: '/' }
              ]
            }
        },
        methods: {}
    }
</script>

<style lang="scss">

</style>
