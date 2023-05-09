<template>
  <NavBar />

  <div class="entries-container">

    <div>
      <EntryList />
    </div>

    <div>
      <router-view />
    </div>

  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
  components: { 
    NavBar: defineAsyncComponent(() => import('../components/NavBar.vue')) ,
    EntryList: defineAsyncComponent(() => import('../components/EntryList.vue')) ,
  },

}
</script>

<style scoped>
.entries-container{
    display: grid;
    grid-template-columns: 1fr 2fr;
    padding: 10px;
    gap: 1rem;
}
</style>