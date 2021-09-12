<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Jules"
      subtitle="The Vale of Belvoir dog walker"
      image="/uploads/frostyfield.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Happy dogs</h3>
       
          <p>
            Hello, I’m Jules
</p>
<p>
I am an independent dog walker in the Vale Of Belvoir. I also offer day care, over night stays and pop in visits, tailored to meet your dog's individual needs.
</p>
<p>
I have a dog of my own called Ernie. He is a friendly and lively red cocker spaniel who loves to socialise with other dogs and is a much loved member of the family!
          </p>

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
