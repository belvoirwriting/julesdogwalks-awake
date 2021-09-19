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
<p>
     ## Walks

| Option                              | Price                                         |
| ----------------------------------- | --------------------------------------------- |
| Group (3 dogs max per group)- 1 hr  | £12 (£3 for additonal dog from same household |
| Solo - 30 min                       | £8                                            |
| Solo - 1 hr                         | £15                                           |
| Solo twice daily - 30min each walk  | £14                                           |

 <i>Weekend and holiday surcharge - £3</i>
</p>
<p>
     ## Day care

| Option                             |Price                                        |
| -----------------------------------|---------------------------------------------|
| All day stay (8 hrs)               |£20 per day                                  |
<i>Weekend and holiday surcharge - £3</i>
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
