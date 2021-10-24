<template>
  <div class="layout--default">
    <section class="main-content columns">
      <aside class="column is-2 section">
        <Sidebar />
      </aside>
      <div class="container column is-10">
        <Nuxt />
      </div>
    </section>
  </div>
</template>

<script>
import Sidebar from "~/components/Sidebar/Sidebar";

export default {
  components: {
    Sidebar
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
.layout--default {
  position: relative;
}
</style>
