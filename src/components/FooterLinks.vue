<template>
<div class="footer">
    <div class="footerLinks uk-position-bottom-center">
        <vk-icon-button v-for="footerLink in footerLinks" 
                        :key="footerLink.id" 
                        v-bind:href="footerLink.url" 
                        v-bind:icon="footerLink.iconName" 
                        v-bind:class="footerLink.className">
        </vk-icon-button>
    </div>
    <span class="copyiright uk-position-bottom-right uk-margin-small-right uk-margin-small-bottom">&copy; {{ calculateDate() }} {{ copyright }}</span>
</div>
</template>

<script>

export default {
  name: 'FooterLinks',
  data () {
    return {
        copyright: 'Alle rechten voorbehouden. Website door Zowie van Geest.',
        footerLinks: [
            {url: 'https://www.linkedin.com/in/zowie-van-geest-9b76864b/', iconName: 'linkedin', className: 'uk-margin-small-right uk-margin-small-bottom'},
            {url: 'https://github.com/zowievangeest', iconName: 'github', className: 'uk-margin-small-right uk-margin-small-bottom'},
            {url: 'https://www.facebook.com/zowie93', iconName: 'facebook', className: 'uk-margin-small-bottom'}
        ] 
    }
  },
  methods: {
      calculateDate: function() {
          return (new Date()).getFullYear();
      }
  }
}
</script>

<style scoped lang="scss">
.uk-icon {
    color: #999;
    background: none;
    border: 1px solid #999;
    transition: color .2s, background .2s, border .2s;
    &:hover {
        background: none;
        color: #05adff;
        border: 1px solid #05adff;
        transition: color .2s, background .2s, border .2s;
    }
}
</style>
