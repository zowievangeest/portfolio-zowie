<template>
  <div id="app" class="background imgloaded">
    <div class="content">
			<div class="glitch">
				<div class="glitch__img"></div>
				<div class="glitch__img"></div>
				<div class="glitch__img"></div>
				<div class="glitch__img"></div>
				<div class="glitch__img"></div>
			</div>
		</div>
    <router-view/>
  </div>
</template>

<style lang="scss">
// Custom Zowie
@import "./assets/scss/main";
@import "./assets/scss/colors";
@import "./assets/scss/glitch";
</style>
