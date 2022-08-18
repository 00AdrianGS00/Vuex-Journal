<template>
  <div class="d-flex justify-content-center">
    <h1 class="align-self-center">No hay nada seleccionado</h1>
  </div>
    <compFab />
</template>

<script>
import { defineAsyncComponent } from "vue";

export default {
  components: {
    compFab: defineAsyncComponent(() => import('../components/compFab.vue'))
  }
}
</script>

<style lang="scss" scoped>

    div {
        height: 100%;
    }

</style>