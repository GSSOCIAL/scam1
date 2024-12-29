<template>
  <div class="application">
    <Header />
    <div class="applicationContainer">
      <slot />
    </div>
  </div>
</template>

<style lang="scss">
body {
  margin: 0px;
  -webkit-font-smoothing: antialiased;
  background-color: var(--background);
  color: var(--color);
  font-size: var(--fontSize);
  font-weight: var(--fontWeight);
  line-height: var(--lineHeight);
  * {
    position: relative;
    box-sizing: border-box;
  }
  a {
    color: var(--link);
  }
  .application {
    &Container {
    }
  }
}
</style>