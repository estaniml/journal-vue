<template>
  <div>
    <h1>No hay nada seleccionado weon</h1>
    <FabBtn />
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'


export default {
    components: {
        FabBtn: defineAsyncComponent(() => import('../components/FabBtn.vue')) ,
    }
}
</script>

<style lang="scss" scoped>

</style>