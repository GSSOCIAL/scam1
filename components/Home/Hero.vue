<template>
  <div class="hero">
    <div class="heroOverlay"></div>
    <div class="heroWrapper">
      <NuxtLink to="/">
        <div class="heroWrapperItem">коттеджи</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">бани</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">бани</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">ресторан</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">мероприятия</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">рыбалка</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">детям</div>
      </NuxtLink>
      <NuxtLink to="/">
        <div class="heroWrapperItem">о клубе</div>
      </NuxtLink>
    </div>
  </div>
</template>


<style scoped lang="scss">
.hero {
  width: 100vw;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-end;
  &Overlay {
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
  }
  &Wrapper {
    display: flex;
    flex-direction: row;
    padding: var(--wrapperV) var(--wrapperH);
    height: 100%;
    width: 100%;
    max-height: 300px;
    flex: 1;
    justify-content: flex-end;
    align-items: stretch;
    a {
      text-decoration: none;
      width: 100%;
      //TODO: Make wave here
      &:nth-child(2n) {
        .heroWrapperItem:before {
          height: 200px;
        }
      }
      &:nth-child(3n + 1) {
        .heroWrapperItem:before {
          height: 60px;
        }
      }
    }
    &Item {
      width: 100%;
      height: 100%;
      padding: 24px 12px 0px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      justify-content: flex-end;
      &:before {
        content: "";
        display: block;
        position: absolute;
        width: 1px;
        bottom: 0px;
        left: 0px;
        transition: 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275) height;
        background: #fff;
        height: 100px;
      }
      &:hover {
        &:before {
          height: 300px !important;
        }
      }
    }
  }
}
</style>