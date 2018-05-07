<template>
  <div class="home">
    <ComingSoon/>
    <FooterLinks/>
  </div>
</template>

<script>
// @ is an alias to /src
import ComingSoon from '@/components/ComingSoon.vue'
import FooterLinks from '@/components/FooterLinks.vue'

export default {
  name: 'home',
  components: {
    ComingSoon,
    FooterLinks
  }
}
</script>
