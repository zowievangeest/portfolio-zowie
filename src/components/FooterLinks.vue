<template>
  <div class="footerLinks uk-position-bottom-center">
    <vk-iconnav>
        <vk-iconnav-item v-for="footerLink in footerLinks" :key="footerLink.id" v-bind:href="footerLink.url" v-bind:icon="footerLink.iconName"></vk-iconnav-item>
    </vk-iconnav>
  </div>
</template>

<script>
export default {
  name: 'FooterLinks',
  data () {
      return {
         footerLinks: [
             {url: 'https://www.linkedin.com/in/zowie-van-geest-9b76864b/', iconName: 'linkedin'},
             {url: 'https://www.linkedin.com/in/zowie-van-geest-9b76864b/', iconName: 'github'},
             {url: 'https://www.linkedin.com/in/zowie-van-geest-9b76864b/', iconName: 'facebook'}
         ] 
      }
  }
}
</script>

<style scoped lang="scss">

</style>
