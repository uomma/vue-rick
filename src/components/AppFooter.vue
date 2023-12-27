<script>
import { store } from '../store';

    export default {
        data(){
            return{
                store
            }
        }
    }
</script>
<template>
<footer class="text-center my-5">
    risultati trovati : {{ store.charactersFound }}
</footer>
</template>



<style lang="scss" scoped>

</style>