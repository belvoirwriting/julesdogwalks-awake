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
<h2>Walks</h2>

<table>
<thead>
<tr>
<th>Option</th>
<th>Price</th>
</tr>
</thead>
<tbody>
<tr>
<td>Group (3 dogs max per group)- 1 hr</td>
<td>£12 (£3 for additonal dog from same household</td>
</tr>
<tr>
<td>Solo - 30 min</td>
<td>£8</td>
</tr>
<tr>
<td>Solo - 1 hr</td>
<td>£15</td>
</tr>
<tr>
<td>Twice daily - 30min each walk</td>
<td>£14</td>
</tr>
</tbody>
</table>
<br/>
</p>
<p>
<h2>Day care</h2>

<table>
<thead>
<tr>
<th>Option</th>
<th>Price</th>
</tr>
</thead>
<tbody>
<tr>
<td>All day stay (8 hrs)  </td>
<td>£20 per day</td>
</tr>
</tbody>
</table>
<br/>
</p>
<p>
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
