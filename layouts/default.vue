<template>
  <div>
    <Nuxt />
  </div>
</template>

<style lang="scss">
html {
  font: {
    family: $font-text, -apple-system, BlinkMacSystemFont, sans-serif;
    size: 16px;
  };
  color: $light-grey;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

body {
  background-color: $dark-grey;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
