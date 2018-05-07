<template>
  <div class="comingsoon uk-height-1-1">
    <div class="uk-vertical-align uk-text-center uk-height-1-1">
      <div class="uk-vertical-align-middle">
        <img class="logo" src="../assets/images/logo-zowie-van-geest.svg" data-uk-svg>
        <h1 class="title uk-text-uppercase">{{ titel }}</h1>
        <p class="description">Portfolio website is under construction, I'm working very hard to give you the best experience with this one.</p>
        <vk-button>More info</vk-button><vk-button>Send mail</vk-button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComingSoon',
  data () {
    return {
      titel: 'coming soon'
    }
  }
}
</script>

<style scoped lang="scss">
.comingsoon {
  .logo {
    width: 125px;
  }
  .title { 
    font-size: 48px;
    letter-spacing: .3em;
    padding: 0 0 0 .3em;
    font-weight: 100;
  }
  .description {
    line-height: 2.5em;
    letter-spacing: .15em;
  }
}
</style>
