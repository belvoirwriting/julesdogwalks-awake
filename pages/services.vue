<template>
  <div id="services-page" class="page-wrapper services-page content-page">
    <site-hero
      title="Services"
      subtitle="Walking happy dogs"
      image="/uploads/happydogs.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>List of service</h3>
       
          <p>
            Coming soon
</p>

<p>
Check back here for our list of services          </p>

        </div>
      </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
