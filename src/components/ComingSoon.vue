<template>
  <div class="comingsoon uk-position-center uk-margin-medium">
    <div class="uk-vertical-align uk-text-center uk-text-white">
      <div class="uk-vertical-align-middle">
        <img class="logo uk-text-white uk-margin-medium-bottom" src="../assets/images/logo-zowie-van-geest.svg" data-uk-svg>
        <h1 class="title uk-text-uppercase uk-text-white uk-margin-medium-bottom">{{ titel }}</h1>
        <p class="description uk-margin-medium-bottom">{{ description }}</p>
        <div class="buttons">
          <a id="more-info" :href="linkedIn" class="btn btn-round btn-solid">More info</a>
          <a id="send-mail" :href="`mailto:${email}`" class="btn btn-round btn-ghost">Send email</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ComingSoon',
  data () {
    return {
      email: 'zowie@zowievangeest.nl',
      linkedIn: 'https://www.linkedin.com/in/zowie-van-geest-9b76864b/',
      titel: "coming soon",
      description: "Portfolio website is under construction, I'm working very hard to give you the best experience with this one."
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
    font-weight: 400;
  }
  .description {
    line-height: 2.5em;
    letter-spacing: .15em;
    font-weight: 100;
  }
  .buttons {
    text-align: center;
  }
}
</style>
