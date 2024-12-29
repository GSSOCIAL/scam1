<template>
  <div class="contentBlock">
    <div class="contentBlockL">
      <slot name="l"></slot>
    </div>
    <div class="contentBlockR">
      <slot name="r"></slot>
    </div>
  </div>
</template>


<style scoped lang="scss">
.contentBlock {
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: flex-start;
  padding: var(--wrapperV) var(--wrapperH);
  gap: var(--gap);
  &L {
    width: 100%;
  }
  &R {
    width: 100%;
  }
}
</style>