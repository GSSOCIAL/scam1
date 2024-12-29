<template>
  <div class="contentTitle">
    <h1><slot /></h1>
  </div>
</template>


<style scoped lang="scss">
.contentTitle {
  padding: var(--wrapperV) var(--wrapperH);
  border-bottom: 1px solid #997c4c;
  h1 {
    max-width: 400px;
  }
}
</style>