<template>
  <section class="links_socialmedia">
    <a v-for="profile in profiles" :key="profile.label" :href="profile.href" target="_blank" :class="profile.linkClass"><i :class="profile.icon" /><span class="link__label">{{ profile.label }}</span></a>
  </section>
</template>

<script>
export default {
  data () {
    return {
      profiles: [
        {
          href: 'https://soundcloud.com/simonamiot',
          linkClass: 'link_block link__branded--soundcloud',
          icon: 'fab fa-soundcloud',
          label: 'Soundcloud'
        },
        {
          href: 'https://twitter.com/simon_amiot',
          linkClass: 'link_block link__branded--twitter',
          icon: 'fab fa-twitter',
          label: 'Twitter'
        },
        {
          href: 'https://www.linkedin.com/in/simon-amiot-894542119/',
          linkClass: 'link_block link__branded--linkedin',
          icon: 'fab fa-linkedin',
          label: 'LinkedIn'
        }
      ]
    }
  }
}
</script>

<style lang="scss">
.links_socialmedia {
  display: flex;
  flex-flow: row wrap;
  @media screen and (max-width: 960px) {
   flex-flow: column nowrap;
  }
  padding: 2rem;
}

.link_block {
  display: inline-flex;
  align-items: center;
  @media screen and (max-width: 640px) {
    font-size: ms(1);
  }
  font-weight: 300;
  padding: 1rem 2rem;
}

i.fab {
  margin: 0 1rem;
  font-size: ms(2);
}
</style>
