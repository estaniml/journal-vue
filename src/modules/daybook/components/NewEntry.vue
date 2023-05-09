<template>
  <div
    @click="$router.push({ name: 'entry', params: { id: 10 }})"
    class="new-entry"
    >
    <div>
        <span>16</span>
        <span>Julio</span>
        <span>2023</span>
    </div>

    <div>
        Este curso tiene por objetivo enseñarte Vue.js desde cero, pero si tu eres alguien que conoce el framework, de igual manera te servirá mucho ya que rápidamente despegaremos en conceptos fundamentales como las pruebas automáticas, Vuex y el nuevo composition api.
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.new-entry{
    background-color: #090909;
    padding: 1rem;
    display: flex;
    flex-direction: column;
    gap: 0.5rem;

    > div {
      background-color: transparent;
    }

    span {
      background-color: transparent;
      color: #ababab;
    }
}
</style>