<template functional>
  <main
    class="base-page"
    :class="`base-page--${pageName}`"
  >
    <div class="container">
      <slot />
    </div>
  </main>
</template>

<script>
export default {
  props: ['pageName']
}
</script>

<style lang="scss">
.base-page {
  padding-top: 20px;
  padding-bottom: 60px;
  @include tablet-only {
    padding-top: 20px;
    padding-bottom: 20px;
  }
  @include mobile {
    padding-top: 16px;
    padding-bottom: 16px;
  }
}
</style>
