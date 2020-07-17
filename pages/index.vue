<template>
  <main class="main">
    <section class="bumper">
      <DischargeCircles />
      <div class="bumper__text">
        <DischargeLogo />
        <!-- <h1 class="bumper__text__pseudonyme">Discharge</h1> -->
        <h2 class="bumper__text__name">Simon Amiot</h2>
        <p class="bumper__text__message">Website under construction</p>
      </div>
    </section>
    <section class="demoreel">
      <h2>Demoreel Mid 2020</h2>
      <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/438985378?color=E6E6Ef&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
    </section>
    <SocialLinks />
  </main>
</template>

<script>
export default {}
</script>

<style lang="scss">
.main {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}
.bumper {
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  height: 100vh;
  width: 100%;
  margin-bottom: 10rem;
  &__text {
    display: flex;
    align-items: center;
    flex-flow: column nowrap;
     &__pseudonyme {
    font-family: $font-display;
    font-size: ms(7);
    }
    &__name {
      @extend h2;
      text-transform: uppercase;
    }
    &__message {
      font-weight: 300;
      font-style: italic;
      font-size: ms(2);
      color: $color-2-darker;
    }
  }
}

.demoreel {
  display: flex;
  flex-flow: column;
  width: 60rem;
  padding: 4rem 0;
}
</style>
