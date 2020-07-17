<template>
  <section class="links_socialmedia">
    <a v-for="profile in profiles" :key="profile.label" :href="profile.href" target="_blank" :class="profile.linkCLass"><i :class="profile.icon" /><span class="link__label">{{ profile.label }}</span></a>
  </section>
</template>

<script>
export default {
  data () {
    return {
      profiles: [
        {
          href: 'https://soundcloud.com/simonamiot',
          linkClass: 'link__branded--soundcloud',
          icon: 'fab fa-soundcloud',
          label: 'Soundcloud'
        },
        {
          href: 'https://twitter.com/simon_amiot',
          linkClass: 'link__branded--twitter',
          icon: 'fab fa-twitter',
          label: 'Twitter'
        },
        {
          href: 'https://www.linkedin.com/in/simon-amiot-894542119/',
          linkClass: 'link__branded--linkedin',
          icon: 'fab fa-linkedin',
          label: 'LinkedIn'
        }
      ]
    }
  }
}
</script>
