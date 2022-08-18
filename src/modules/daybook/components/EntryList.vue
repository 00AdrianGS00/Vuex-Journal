<template>
    <div class="entry-list-container">
        <div class="px-2 pt-2">
            <input type="text"
                   class="form-control"
                   placeholder="Buscar Entradas" >
        </div>
        <div class="entry-scrollarea">
            <h2 v-for="item in 100"
                :key="item">
                <compEntry />
            </h2>
        </div>
    </div>    
</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
    components: {
        compEntry: defineAsyncComponent(() => import('./compEntry.vue'))
    },
    
}
</script>

<style lang="scss" scoped>

    input{
        height: 25px;
    }

    .entry-list-container {
        border-right: 1px solid #2C3E50;
        height: calc( 100vh - 56px );

    }

    .entry-scrollarea {
        height: calc(100vh - 120px);
        overflow: scroll;
    }
</style>