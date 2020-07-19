<template>
  <main class="main">
    <section class="bumper">
      <DischargeCircles />
      <div class="bumper__text">
        <DischargeLogo />
        <!-- Clean this in future commit -->
        <!-- <h1 class="bumper__text__pseudonyme">Discharge</h1> -->
        <h2 class="bumper__text__name">
          Simon Amiot
        </h2>
        <p class="bumper__text__message">
          Website under construction
        </p>
      </div>
      <div class="bumper__scroll-CTA">
        <p>Scroll to see the demoreel</p>
        <i class="fas fa-arrow-down" />
      </div>
    </section>
    <section class="demoreel">
      <!-- Clean this in future commit -->
      <h2>
        Demoreel Mid 2020
      </h2>
      <div class="demoreel__video" style="padding:70% 0 0 0;position:relative;">
        <iframe src="https://player.vimeo.com/video/438985378?color=E6E6Ef&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="fullscreen" allowfullscreen />
      </div>
    </section>
    <SocialLinks />
  </main>
</template>

<style lang="scss">
.main {
  display: flex;
  flex-flow: column nowrap;
  align-items: center;
}
.bumper {
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-content: center;
  align-items: center;
  height: 100vh;
  width: 100%;
  margin-bottom: 10rem;
  &__text {
    display: flex;
    max-width: 60rem;
    width: 100%;
    align-items: center;
    flex-flow: column nowrap;
    margin-top: 14rem;
    margin-bottom: 8rem;
     &__pseudonyme {
    font-family: $font-display;
    font-size: ms(7);
    width: 100%
    }
    &__name {
      @extend h2;
      text-align: center;
      text-transform: uppercase;
    }
    &__message {
      font-weight: 300;
      font-style: italic;
      font-size: ms(2);
      text-align: center;
      color: $color-2-darker;
    }
  }
  &__scroll-CTA {
    text-align: center;
    p {
      font-size: ms(2);
      font-weight: 300;
      font-style: italic;
      margin-bottom: 2rem;
    }
    i.fa-arrow-down {
      font-size: ms(3);
    }
  }
}

// Clean this in future commit
.demoreel {
  display: flex;
  flex-flow: column;
  max-width: 60rem;
  margin: 2rem 0;
  // Clean this in future commit
  &__video {
    width: 100%;
  }
  h2 {
    text-align: center;
  }
}
</style>
