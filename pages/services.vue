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
<td>Group walk (3 dogs max per group)- 1 hr</td>
<td>£12 (£3 for additional dog from same household)</td>
</tr>
<tr>
<td>Solo walk - 30 min</td>
<td>£8</td>
</tr>
<tr>
<td>Solo walk - 1 hr</td>
<td>£15</td>
</tr>
<tr>
<td>Twice daily walks - 30min each</td>
<td>£14</td>
</tr>
<tr>
<td>Weekend and holiday surcharge</td>
<td>£3</td>
</tr>
</tbody>
</table>
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
<td>All day stay (8 hrs)</td>
<td>£20 per day</td>
</tr>
</tbody>
</table>
<br/>
</p>
<p>
<h2>Overnight stays</h2>

<table>
<thead>
<tr>
<th>Option</th>
<th>Price</th>
</tr>
</thead>
<tbody>
<tr>
<td>Overnight stay (24 hrs)</td>
<td>£25 per night</td>
</tr>
</tbody>
</table>
<br/>
</p>

<h2>Home visits / pop-ins</h2>
Perfect for pups, older dogs, cats and other small animals
<table>
<thead>
<tr>
<th>Option</th>
<th>Price</th>
</tr>
</thead>
<tbody>
<tr>
<td>20 min visit - feeding, toilet break, cuddles</td>
<td>£8</td>
</tr>
<tr>
<td>Twice daily visit</td>
<td>£14</td>
</tr>
<tr>
<td>Weekend and holiday surcharge</td>
<td>£3</td>
</tr>
</tbody>
</table>
<br/>
</p>

<h2>Pet taxi</h2>
Transport to vet or groomers
<table>
<thead>
<tr>
<th>Option</th>
<th>Price</th>
</tr>
</thead>
<tbody>
<tr>
<td>Per trip</td>
<td>£10 plus 50p per mile</td>
</tr>
<tr>
<td>Waiting times</td>
<td>£5 per 15 min</td>
</tr>
</tbody>
</table>
<br/>
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
      title: `Services | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
