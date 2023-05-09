<template>
  <div style="width: 100%">
    <input  
        type="text"
        placeholder="Buscar..."
    />

    <div>
        <div class="entries-container">
            <NewEntry
                v-for="item in 100"
                :key="item"
            />
        </div>
    </div>
  </div>
</template>

<script>
import { defineAsyncComponent } from 'vue'

export default {
    components: { 
    NewEntry: defineAsyncComponent(() => import('./NewEntry.vue')),
  },
}
</script>

<style lang="scss" scoped>
.entries-container{
    display: flex;
    flex-direction: column;
    gap: 1rem;
}

input {
    border: 1px solid rgb(255, 255, 255);
    outline: none;
    padding: 5px;
    width: 100%;
    margin-bottom: 1rem;
    border-radius: 5px;

    &:focus{
        outline: none;
    }
}
</style>