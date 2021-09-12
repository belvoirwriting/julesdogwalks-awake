<template>
  <footer class="site-footer">
<b>Email</b> julesdogwalks@gmail.com
 <br />

   
   Dog walker based in Granby, Nottingham, walking dogs from villages across the Vale of Belvoir, offering day care and overnight stays for your dog.
<br /> 
{{ $siteConfig.siteName }} &copy; {{ new Date().getFullYear() }} - All
    Rights Reserved
  </footer>
</template>

<script>
export default {
  name: 'SiteFooter'
}
</script>

<style scoped>
footer {
  background: #eee;
  padding: 20px 10px;
  text-align: center;
  transition: 0.5s ease all;
}
</style>
