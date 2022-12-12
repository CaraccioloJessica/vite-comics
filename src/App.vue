<script>
import AppHeader from './components/AppHeader.vue'
import InfoSection from './components/InfoSection.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    InfoSection,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <main>

  </main>
  <footer>
    <InfoSection />
    <AppFooter />
  </footer>
  <main>

  </main>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/_variables' as *;

body {
  background-color: $black_dc;
}
</style>
