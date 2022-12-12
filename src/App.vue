<script>
import AppHeader from './components/AppHeader.vue'
import InfoSection from './components/InfoSection.vue'
import AppFooter from './components/AppFooter.vue'
import SocialSection from './components/SocialSection.vue'

export default {
  components: {
    AppHeader,
    InfoSection,
    AppFooter,
    SocialSection
  }
}
</script>

<template>
  <AppHeader />

  <main>

  </main>

  <footer>
    <section>
      <InfoSection />
    </section>

    <section>
      <AppFooter />
    </section>

    <section>
      <SocialSection />
    </section>
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
